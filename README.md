# apigee-devportal-wsdl-docs
Sample to load WSDL docs to Apigee dev portal (Drupal)

## Pre-req:
- Apigee Edge account
- Apigee Dev portal (Drupal)
	- Installed [wsdl_docs](https://cgit.drupalcode.org/wsdl_docs/tree/README.txt) module
- Maven 3.x or later
- Java 8 or later


## Steps:
- Execute `mvn process-resources -Dportal.auth="{portal.auth}" -Dportal.url="{portal.url}" -Dwsdl_name="{wsdl_name}" -Dpath_to_wsdl_directory="{path_to_wsdl_directory}" -Dwsdl_file_name="{wsdl_file_name}"`
- Should be seeing the new doc in the portal if everything is good

NOTE: The pom also makes a `cat` command call to print the output. If your OS does not support this, please change it or comment the plugin
