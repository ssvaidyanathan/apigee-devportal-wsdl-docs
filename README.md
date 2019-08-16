# apigee-devportal-wsdl-docs
Sample to load WSDL docs to Apigee dev portal (Drupal)

## Pre-req:
- Apigee Edge account
- Apigee Dev portal (Drupal)
	- Installed [wsdl_docs](https://git.drupalcode.org/project/wsdl_docs) module
- Maven 3.x or later
- Java 8 or later


## Steps:
- Execute `mvn process-resources -Dportal.username="{portal.username}" -Dportal.password="{portal.password}" -Dportal.url="{portal.url}" -Dservice_name="{service_name}" -Dwsdl_file="{wsdl_file_full_path}`
- Should be seeing the new doc in the portal if everything is good
