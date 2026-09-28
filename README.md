© The Chancellor, Masters and Scholars of The University of Oxford. All rights reserved.

# Explore different providers

This course is available for multiple cloud providers. Choose your preferred platform:

- [Hello Google Cloud](https://github.com/Oxford-Research-Cloud-Competency-Centre/Hello-gcloud) 
- [Hello Microsoft Azure](https://github.com/Oxford-Research-Cloud-Competency-Centre/Hello-azure)
- [Hello Amazon Web Services](https://github.com/Oxford-Research-Cloud-Competency-Centre/Hello-aws) (⭐ Most popular)
- [Hello IBM Cloud](https://github.com/Oxford-Research-Cloud-Competency-Centre/Hello-ibm-cloud) (You are here)

# Instructions

<details>
<summary>Create a new container registry namespace called hello-registry in region eu-gb</summary>


***
</details>
<details>
<summary>Create a new serverless project called hello-project in region eu-gb</summary>

***
</details>
<details>
<summary>Create a new application called hello-ibm-cloud</summary>


***
</details>
<details>
<summary>Select "Build container image from source code" then press "Specify build details"</summary>

***
</details>
<details>
<summary>Set the source to https://github.com/Oxford-Research-Cloud-Competency-Centre/Hello-ibmcloud</summary>

***
</details>
<details>
<summary>Set the strategy to Cloud Native Buildpack</summary>


***
</details>
<details>
<summary>Set the output to hello-ibm-cloud in hello-registry using a Code Engine Managed Secret in the London region</summary>

***
</details>
</details>
<details>
<summary>Change the default port from 8080 to 80</summary>

***
</details>
<details>
<summary>Find the public URL</summary>

***
</details>
<details>
<summary>Test the app</summary>

***
</details>

# Going further

<details>
<summary><h2>Adding an API endpoint</h2></summary>

Add the following code in app.py

```	
@app.route("/hello_api")
def hello_api():
    return {
		"name": "Wrinkle Five Star",
		"species": "Duck",
		"breed": "American Pekin",
		"hatching_date": "2020-09-09",
		"sex": "Male"
    }
```

Then test your endpoint

</details>

<details>
<summary><h2>Local testing</h2></summary>

You need to test your changes before publishing them. 

<details>
<summary>Install Python</summary>

```	
https://www.python.org/downloads/
```

***
</details>
<details>
<summary>Install dependencies</summary>

```	
python -m pip install --break-system-packages -r requirements.txt
```

***
</details>
<details>
<summary>Run flask</summary>

```	
python -m flask run --port=80
```

Open localhost in your browser.   

***
</details>

</details>

<details>
<summary><h2>Cleaning up</h2></summary>

<details>
<summary>To find and delete all active resources, go to cloud.ibm.com/resources</summary>

***
</details>

<details>
<summary>You can then go to Manage / Access (IAM) and delete any remnant for example this service ID</summary>

***
</details>

</details>
