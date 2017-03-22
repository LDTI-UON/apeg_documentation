## Configuration

To configure the tool, access on the LTI link created earlier (ensure you are not in preview mode).

## Activate peer assessment
_This feature is primarily for developers and will be removed in future releases_

![Activate Peer Assessment](images/bb_activate_pa.png )

### Manually Upload the Student Gradebook

To manually upload the student list, first download the [student list from group export](https://en-us.help.blackboard.com/Learn/Instructor/Interact/Course_Groups/080_Import_and_Export_Groups). Ensure you select the _Groups and group members_ and _Include header row_ options. The file will be emailed to you. You will need to download it from the link in the email.

![Export Groups](images/bb_export_groups.png)

In the instructor view, uploadt the csv file using the form.

![Manual Upload](images/bb_upload_student_list.png)

## Add a Rubric ##

[Export a rubric from Blackboard Learn](https://en-us.help.blackboard.com/Learn/Instructor/Grade/Rubrics#Import_and_export_rubrics) that you would like the students to use to assess each other.

![Export a Rubric](images/bb_export_rubric.png)

Upload the rubric ZIP file into the peer review tool using the form:
![Upload a Rubric](images/bb_upload_rubric.png)

Select the rubric from the dropdown and Attach. You can use Preview to preview the Rubric.

_Rubrics will ***not*** attach automatically, ensure you click Attach._

![Attach a Rubric](images/bb_attach_rubric.png)

## Configure Student View

There are several configuration options for the student view.

* Show grade column
    * _students can see the grade others have given them_
* Show comments
    * _students can see the comments others have given them_
* Turn on self assessment
    * _students assess their own performance first, they cannot assess others until they have assessed themselves_
      * **When changing this setting you will need to resync the user groups (see [Gradebook Syncronisation](#gradebook-syncronisation))**
* Include self in mean score
    * _mean score includes the student's own score, for example if there are 5 in the group and the total score the group has given the student is 300 the final score will be 300/5 = 60 rather than 300/4 = 75_
* Total maximum score for assessment
    * _used to calculate the percentage score, if you are not using a rubric you can set this here. The rubric total
      score will override this setting if a rubric is attached_

![Peer Review Settings](images/bb_pa_settings.png)
