## Steps to generate the forms and email drafts for each employee.

1. Clone this repository.

```
git clone https://github.com/simon3z/mashov
```

2. Create a new project in script.google.com. Name it whatever you want. We have to do this because we are adding some variables that point to directories that we are creating for our teams.

3. Copy the Code.gs into the project.

4. Create a directory on Google Drive to save all the forms in.  Get the ID from that directory.

5. Get the ID from the centralized form and spreadsheet.

Google form ID: 1fs7iGd0rbAw1EX5QOmTrYvsHo9OBkNljCKoYbfSf7BA <br>
Google spreadsheet ID: 1lxaZR2ncek_46x0jNuejyg642_SauAvmqzxCZ9Aw6Fg 

6. Change the variables to meet your needs. See the following for an example (sanitized).

* line 6 - the survey form id
* line 7 - a google drive to store all the feedback forms
* line 10 - the review spreadsheet
* line 15 - email signature

optional:
* line 13 - If U want to have visibility to your managers' feedback forms they need to set it up

7. Run the code to generate the forms and email drafts. In the script.google.com inteface of the project, click on the `Select Function` dropdown, and then select the `GenerateForms` function, click the `Play` button.

8. In the background, the function will generate the forms in your Google drive in the location you specified. It will also generate draft emails (one per reviewer) in your gmail drafts folder. Finally, it will update the spreadsheet that the forms were generated.
