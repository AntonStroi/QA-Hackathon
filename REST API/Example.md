# Test Task, Anton Stroi

Test cases for endpoint {{host}}//pet/{{petId}}  
https://petstore.swagger.io/#/pet/updatePetWithForm

Some test cases include assumptions or comments due to missing requirements in the provided documentation!!!

---

### Test Case № 1:
**Title:** Successful update of the pet's name  

**Description:** Verify that the endpoint correctly replaces the value of the pet's 'name' field with the value ​​passed in the request, leaving other fields of the object unchanged.  

**Preconditions:**  
1) The pet's initial data in the database is as follows  
   id = 123,  
   name = "Mur",  
   status = "available"  

**Steps:**  
1) Send a POST request to {{host}}//pet/123 with parameters:  
   name = "Updated name"  

**Expected Result:**  
1) Status code of the response: 200 OK.  
2) The name field of the pet with ID 123 is updated in the database to "Updated name".  
3) Other fields of the pet remain unchanged.  

---

### Test Case № 2:
**Title:** Updating the name field to a value that is outside the allowed length  

*(Since there are no clear requirements in the Swagger documentation, this test assumes a maximum length of 15 characters for the 'name' field as an example)*  

**Description:** Verify that the Server will return an error when trying to update the name field to a value whose length is greater than the maximum allowed.  

**Preconditions:**  
1) The pet's initial data in the database is as follows  
   id = 123,  
   name = "Mur",  
   status = "available"  

**Steps:**  
1) Send a POST request to {{host}}//pet/123 with the following parameters:  
   name = "Verylongsentence"  

**Expected Result:**  
1) Status code of the response: 400.  
2) The response body contains information about the error, such as:  
   `"The name field exceeds the allowed maximum length."`  

**Comment:** The requirements for this test case should be clarified, as the exact field length limit and error format are not specified in the documentation.  

---
