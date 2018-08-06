# Description :
		
	This repository showcases how to package existing vSphere python script into AWS Lambda Function.

# Instructions :

1. Setup Virtual Environment  
	`py -3.6 -m venv .`

2. Activate Virtual Environment
	
	(Windows) `.\Scripts\activate`

3. Install vSphere SDK

	* Download/Clone vSphere python SDK from this repo : https://github.com/vmware/vsphere-automation-sdk-python
	* Install SDK by running pip : `pip install --upgrade --force-reinstall -r <path to vsphere-automation-sdk-python folder>/requirements.txt -t . --extra-index-url file://<absolute path to sphere-automation-sdk-python folder>/lib`

4. Modify code :
	
	* Download source code from : https://github.com/vmware/pyvmomi/blob/master/sample/poweronvm.py
	* Modify the code to match sample.py or alternatively do the following on sample.py
		* comment line 33-45/ uncomment 47 - 61
		* comment line 116 122 / uncomment 115 121
	
5. Package Lambda
	Follow Instructnions here : https://docs.aws.amazon.com/lambda/latest/dg/lambda-python-how-to-create-deployment-package.html
	