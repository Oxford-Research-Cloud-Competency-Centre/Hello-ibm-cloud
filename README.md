
© The Chancellor, Masters and Scholars of The University of Oxford. All rights reserved.

# Explore different providers

This course is available for multiple cloud providers. Choose your preferred platform:

- [Hello Google Cloud](https://github.com/Oxford-Research-Cloud-Competency-Centre/Hello-gcloud) 
- [Hello Microsoft Azure](https://github.com/Oxford-Research-Cloud-Competency-Centre/Hello-azure)
- [Hello Amazon Web Services](https://github.com/Oxford-Research-Cloud-Competency-Centre/Hello-aws) (⭐ Most popular)
- [Hello IBM Cloud](https://github.com/Oxford-Research-Cloud-Competency-Centre/Hello-ibm-cloud) (You are here)

# Instructions

<details>
<summary>Create a new container registry namespace named hello-registry in region eu-gb</summary>

<img width="1268" height="921" alt="img00" src="https://github.com/user-attachments/assets/82657605-0f14-4f05-9687-830c21edbc0b" />

***
</details>
<details>
<summary>Create a new serverless project named hello-project in region eu-gb</summary>

<img width="1341" height="923" alt="img0" src="https://github.com/user-attachments/assets/133b8ca6-3e30-4c61-b912-a7ec9e799cfd" />

***
</details>
<details>
<summary>Create a new application called hello-ibm-cloud</summary>

<img width="976" height="691" alt="img1" src="https://github.com/user-attachments/assets/91bf4a1d-753f-430f-bfb0-d52fafeb9198" />

***
</details>
<details>
<summary>Select "Build container image from source code" then press "Specify build details"</summary>

<img width="1123" height="376" alt="img2" src="https://github.com/user-attachments/assets/ecf88a9c-b5c2-4439-9b05-878d5ce5e96b" />

***
</details>
<details>
<summary>Set the source to https://github.com/Oxford-Research-Cloud-Competency-Centre/Hello-ibmcloud</summary>

<img width="572" height="922" alt="img3" src="https://github.com/user-attachments/assets/8c83a88f-f7ea-41c1-b8ee-43fe9f1ea5f4" />

***
</details>
<details>
<summary>Set the strategy to Cloud Native Buildpack</summary>

<img width="572" height="922" alt="img4" src="https://github.com/user-attachments/assets/e89c263c-ef0b-43d8-a89d-d76e86726c81" />

***
</details>
<details>
<summary>Set the output to hello-ibm-cloud in hello-registry using a Code Engine Managed Secret in the London region</summary>

<img width="532" height="743" alt="img5" src="https://github.com/user-attachments/assets/1362c101-4329-4b97-a24b-9318adf1e866" />

***
</details>
</details>
<details>
<summary>Change the default listening port from 8080 to 80</summary>

<img width="390" height="399" alt="img10" src="https://github.com/user-attachments/assets/6361e7f5-7cc8-49a5-a619-4ad46f603ae3" />

***
</details>
<details>
<summary>Find the public URL</summary>

<img width="1128" height="697" alt="img12" src="https://github.com/user-attachments/assets/edd4c3ef-e4d0-4937-89ea-cf941310154c" />

***
</details>

Test the app

<img width="729" height="222" alt="img8" src="https://github.com/user-attachments/assets/886a2164-e0d3-4516-98c4-7200fb58df53" />


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

<img width="973" height="305" alt="img11" src="https://github.com/user-attachments/assets/aca673e1-6536-4427-b043-ef2826787890" />


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

</details>

Open localhost in your browser.  

<img width="458" height="243" alt="img9" src="https://github.com/user-attachments/assets/1ce97f65-3845-45ef-8ca6-5a59603b159f" />

***

</details>

<details>
<summary><h2>Cleaning up</h2></summary>

<details>
<summary>To find and delete all active resources, go to cloud.ibm.com/resources</summary>

<img width="1564" height="895" alt="img13" src="https://github.com/user-attachments/assets/28d66895-fa68-4c99-923f-4fd519baf6bf" />

***
</details>

<details>
<summary>You can then go to Manage / Access (IAM) and delete any remnant for example this service ID</summary>

<img width="1908" height="972" alt="img14" src="https://github.com/user-attachments/assets/5e42b9e7-64ab-4291-bfaf-c5c66616fb78" />

***
</details>

</details>
