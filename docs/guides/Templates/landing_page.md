# Landing Page Example Template

``` html
<!DOCTYPE html>
<html>
<head>
    <title>{resource_title}</title>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.3/jquery.min.js"></script>
</head>
<body>
  {exp:learning_tools_integration
    prev_link_url='https://uonline-stg.newcastle.edu.au/images/ci/ng/small_previous.gif'
    next_link_url='https://uonline-stg.newcastle.edu.au/images/ci/ng/small_next.gif'
    first_link_url='https://uonline-stg.newcastle.edu.au/images/ci/ng/small_rewind.gif'
    last_link_url='https://uonline-stg.newcastle.edu.au/images/ci/ng/small_ffwd.gif'
   	plugins='lti_peer_assessment'}
     {css_link_tags}
    <!-- imported from LMS -->
    <style>
    .liItem {
    padding: 25px;
    }
    textarea {
    width: 22em;
    height: 5em;
    }
    table {
    min-width: 90% !important;
    }
    th {
    height: 20px !important;
    /*background-color: gray;*/
    color: white;
    padding: 8px;
    }
    td {
    height: 20px;
    padding: 8px;
    }
    tr:nth-child(odd) {
    background-color: rgb(196, 225, 234);
    }
    /* verification form styles*/
    .p_ver {
    padding: 1.1em;
    }
    .p_ver > input {
    margin-left: 2em;
    }
    .not_matched {
    background-color: rgb(200, 155, 180);
    }
    </style>
    {if error_messages != ""}
    	{error_messages}
    {/if}
 	{if logged_in}
    <div class='locationPane'>
        <div class='contentPane'>
            <div class='pageTitle clearfix'>
                <h1>{resource_title}</h1>
                <p>{resource_link_description}</p>
                <p><span class='warningMsg'>{general_message}</span></p>
                <p><a href='{launch_presentation_return_url}'>Return to course:
                {course_name}</a></p>
            </div>
            <div class='contentBox clearfix'>
                <ul>
                    <li class='clearfix liItem'>{if is_instructor == 1}
                    	               <h1>General Settings</h1>
               <p>Group import &amp; Plugin settings</p>
               <hr />
              	<br />
              	{general_settings_form}
              <hr/>
              <br/>

                        <h1>Students registered for Peer Evaluation</h1>
                        <div class='datalist' style='display: inline-block'>
                            {student_table}
                        </div>
                        <h3>Give Students Access to Peer Evaluation</h3>
                        <p>{upload_student_list}</p>
                        <h3>Blackboard Rubrics</h3>
                        <p>Upload rubrics here for this course, attached
                        rubrics will be used by students to grade their
                        peers.</p>
                        <p><em>To create and export a rubric from Blackboard,
                        go to <strong>Organisation Tools &rarr;
                        Rubrics</strong>.</em></p><br>
                        <h4>Upload a rubric</h4>
                        <p>{upload_blackboard_rubric}</p>
                    </li>
                    <li class='clearfix liItem'>
                        <h2>Further Tools</h2>
                        <h3>Settings</h3>{exp:lti_peer_assessment:settings}
                        <hr>
                        <br>
                        <h3>Download Evaluations</h3>
                        <h4><em>Download Evaluations as Excel Spreadsheet</em></h4>{exp:lti_peer_assessment:download_excel}
                    </li>
                    <li style="list-style: none">{if:else}
                        <h1>{exp:lti_peer_assessment:group_name}</h1>
                        <h2>Your Evaluations of Other Group Members</h2>
                        <h3>Evaluation Form</h3>
                        <p style='font-size: 1.5em'><a href='https://bold-space.newcastle.edu.au/lti/index.php/cmns3530/marking_impact'>Access this link for the Marking Impact document</a></p><br>
                        {exp:lti_peer_assessment:form type='single'}
                        {/if}
                    </li>
                    <li class='liItem clearfix'>
                        <p><a href='{launch_presentation_return_url}'>Return to
                        course: {course_name}</a></p>{/if}
                    </li>
                </ul>
            </div>
        </div>
    </div>
    {/exp:learning_tools_integration}
</body>
```

</html>
