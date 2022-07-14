- SAP Demo -

A demo showing the SAP connector funcationallity, connecting to the mulesoft demo environment:

	http://sapidp.demos.mulesoft.com:8000/nwbc/?sap-client=800&sap-language=EN&sap-nwbc-node=root&sap-theme=sap_tradeshow_plus

SAP Connector Documentation:

	https://docs.mulesoft.com/sap-connector/5.5/

Setup:

You will need to log into Credentials Repo and add the appropriate username and pass to the config.yaml file in src/main/resources

This demo is already configured to the mulesoft demo account using the SAP connector with a Windows JCo Native Library.  If you want to run it locally on a different
OS or deploy it to Cloudhub, change the JCo Native Library by downloading it from here:

	https://drive.google.com/drive/u/0/folders/1sZ5fUHW-sE-i5Hx98gBVeD3E9KC7psbw?ths=true
	
More documentation on debugging connection issues with the SAP libraries:

	https://salesforce.quip.com/lcD2ALbVKXYh

Creating New BAPI RFCs:

To create a new BAPI call, add the RFC processor and choose the appropriate function from the drop down menu (the magnifying glass).
To get documentation on specific functions you may read the public documentation here:

	https://www.stechno.net/repository/sap-functions.html

or for internal documentation, install the SAP GUI from here:

	https://sites.google.com/a/mulesoft.com/sap/abc/libs-tools
	
Once installed use the following connection string (if using the mulesoft demo instance):

	conn=/H/54.174.74.71/S/3200&clnt=800&user=mule01&lang=en&systemName=IDP
	
Inside the SAP GUI, use the search box to navigate to module se37.  This will take you to the function builder.  Input the name of the
BAPI function you want documentation on.  Press "Display" for the written function.  Further documentation is found in the top right corner
via the "Function Module Documentation" button.
	
