<!DOCTYPE html>
<!-- saved from url=(0218)https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Peer%20Graded%20Assignment%20-%20Part%202/instructions.md.html?origin=www.coursera.org -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="./instructions-2_files/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
    <link rel="stylesheet" href="./instructions-2_files/default.min.css">
  <style type="text/css">/* this file is used for labs on cognitiveclass.ai that were written in markdown */

/* applies to images, i.e. "![]()" in markdown */
img {
  max-width: 100%;
  height: auto;
}

/* add padding and margins */
body {
  padding: 10px;
  margin: 10px;
}

/* applies to tables, i.e. "|--|--|" in markdown */
table td,
table th {
  padding: 0.75rem;
  vertical-align: top;
  border-top: 1px solid #dee2e6;
}

/* applies to using quotes, i.e. ">" in markdown */
blockquote {
  background: #f9f9f9;
  border-left: 10px solid #ccc;
  margin: 1.5em 10px;
  padding: 1em 10px 0.1em 10px;
  quotes: '\201C''\201D''\2018''\2019';
}

/* the headers need some spacing */

h1,
h2,
h3,
h4,
h5,
h6 {
  font-weight: 500;
  padding-top: 20px;
}

/* Add padding between nested list item */
ul > li > ul {
  padding-bottom: 1rem;
}

.code-badge-language {
  display: none;
}
.code-badge-copy-icon {
  background: url('data:image/svg+xml;base64,PHN2ZyBhcmlhLWhpZGRlbj0idHJ1ZSIgZm9jdXNhYmxlPSJmYWxzZSIgZGF0YS1wcmVmaXg9ImZhciIgZGF0YS1pY29uPSJjb3B5IiBjbGFzcz0ic3ZnLWlubGluZS0tZmEgZmEtY29weSBmYS13LTE0IiByb2xlPSJpbWciIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgdmlld0JveD0iMCAwIDQ0OCA1MTIiPjxwYXRoIGZpbGw9ImN1cnJlbnRDb2xvciIgZD0iTTQzMy45NDEgNjUuOTQxbC01MS44ODItNTEuODgyQTQ4IDQ4IDAgMCAwIDM0OC4xMTggMEgxNzZjLTI2LjUxIDAtNDggMjEuNDktNDggNDh2NDhINDhjLTI2LjUxIDAtNDggMjEuNDktNDggNDh2MzIwYzAgMjYuNTEgMjEuNDkgNDggNDggNDhoMjI0YzI2LjUxIDAgNDgtMjEuNDkgNDgtNDh2LTQ4aDgwYzI2LjUxIDAgNDgtMjEuNDkgNDgtNDhWOTkuODgyYTQ4IDQ4IDAgMCAwLTE0LjA1OS0zMy45NDF6TTI2NiA0NjRINTRhNiA2IDAgMCAxLTYtNlYxNTBhNiA2IDAgMCAxIDYtNmg3NHYyMjRjMCAyNi41MSAyMS40OSA0OCA0OCA0OGg5NnY0MmE2IDYgMCAwIDEtNiA2em0xMjgtOTZIMTgyYTYgNiAwIDAgMS02LTZWNTRhNiA2IDAgMCAxIDYtNmgxMDZ2ODhjMCAxMy4yNTUgMTAuNzQ1IDI0IDI0IDI0aDg4djIwMmE2IDYgMCAwIDEtNiA2em02LTI1NmgtNjRWNDhoOS42MzJjMS41OTEgMCAzLjExNy42MzIgNC4yNDMgMS43NTdsNDguMzY4IDQ4LjM2OGE2IDYgMCAwIDEgMS43NTcgNC4yNDNWMTEyeiI+PC9wYXRoPjwvc3ZnPg==');
  background-size: 100% 100%;
}

.code-badge {
  bottom: 0 !important;
  top: unset !important;
  background: unset !important;
}

.code-badge > .code-badge-check-icon {
  background: green;
}
.code-badge-check-icon {
  font-size: 1.2em;
  cursor: pointer;
  padding: 0 7px;
  background: url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGFyaWEtaGlkZGVuPSJ0cnVlIiBmb2N1c2FibGU9ImZhbHNlIiBkYXRhLXByZWZpeD0iZmFzIiBkYXRhLWljb249ImNoZWNrIiBjbGFzcz0ic3ZnLWlubGluZS0tZmEgZmEtY2hlY2sgZmEtdy0xNiIgcm9sZT0iaW1nIiB2aWV3Qm94PSIwIDAgNTEyIDUxMiIgc3R5bGU9IiYjMTA7ICAgIGNvbG9yOiAjMmFmZjMyOyYjMTA7Ij48cGF0aCBmaWxsPSJjdXJyZW50Q29sb3IiIGQ9Ik0xNzMuODk4IDQzOS40MDRsLTE2Ni40LTE2Ni40Yy05Ljk5Ny05Ljk5Ny05Ljk5Ny0yNi4yMDYgMC0zNi4yMDRsMzYuMjAzLTM2LjIwNGM5Ljk5Ny05Ljk5OCAyNi4yMDctOS45OTggMzYuMjA0IDBMMTkyIDMxMi42OSA0MzIuMDk1IDcyLjU5NmM5Ljk5Ny05Ljk5NyAyNi4yMDctOS45OTcgMzYuMjA0IDBsMzYuMjAzIDM2LjIwNGM5Ljk5NyA5Ljk5NyA5Ljk5NyAyNi4yMDYgMCAzNi4yMDRsLTI5NC40IDI5NC40MDFjLTkuOTk4IDkuOTk3LTI2LjIwNyA5Ljk5Ny0zNi4yMDQtLjAwMXoiLz48L3N2Zz4=');
  background-size: 100% 100%;
}
</style></head>
  <body cz-shortcut-listen="true">
    <img src="./instructions-2_files/IDSNlogo.png" width="200" height="200">
    <h1>Peer-Graded Assignment: Final Assignment – Part 2</h1>
    <p><strong>Estimated time needed:</strong> 45 minutes</p>
    <p>You have now completed the first part of this final assignment. In this second part of the final assignment, you will take some cleaned and prepared data and create some pivot tables from it to help you analyze the data.</p>
    <h1>Software Used in this Assignment</h1>
    <p>The instruction videos in this course use the full Excel Desktop version as this has all the available product features, but for the hands-on labs we will be using the free 'Excel for the web' version as this is available to everyone.</p>
    <p>Although you can use the Excel Desktop software if you have access to this version, <ins>it is recommended that you use Excel for the web for the hands-on labs</ins> as the lab instructions specifically refer to this version, and there are some small differences in the interface and available features.</p>
    <h1>Dataset Used in this Assignment</h1>
    <p>The dataset used in this lab comes from the following source: <a href="https://data.montgomerycountymd.gov/Government/Fleet-Equipment-Inventory/93vc-wpdr?utm_medium=Exinfluencer&amp;utm_source=Exinfluencer&amp;utm_content=000026UJ&amp;utm_term=10006555&amp;utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDA0130ENSkillsNetwork20531059-2021-01-01" target="_blank" rel="external">https://data.montgomerycountymd.gov/Government/Fleet-Equipment-Inventory/93vc-wpdr</a> under a <strong>Public Domain license</strong>.</p>
    <p>We are using a modified subset of that dataset for the lab, so to follow the lab instructions successfully please use the dataset provided with the lab, rather than the dataset from the original source.</p>
    <h2>Assignment Scenario</h2>
    <p>In this final assigment, you will be following the scenario of a recently hired Junior Data Analyst in a local government office, who has been tasked with sorting and analyzing fleet inventory data that was previously imported and cleaned. You plan to use pivot tables to analyze the data in preparation for the results to be visualized in a dashboard and added to a data findings report later.</p>
    <h2>Guidelines for the Submission</h2>
    <p>Download and open the <a href="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Peer%20Graded%20Assignment%20-%20Part%202/Montgomery_Fleet_Equipment_Inventory_FA_PART_2_START.xlsx">Montgomery_Fleet_Equipment_Inventory_FA_PART_2_START.XLSX</a> file in Excel for the web.</p>
    <p>Use the course videos from Module 4 and the lab ‘Hands-on Lab 7: Using Pivot Tables’ to help you complete these tasks.</p>
    <p>Tasks to perform:</p>
    <ol>
      <li>
        <p><strong>Format the data as a table:</strong> Use the Format as Table option to format the data as a table.</p>
      </li>
      <li>
        <p><strong>Use AutoSum to calculate values:</strong> Use AutoSum to find the following values for column 'C' and record each of the values:</p>
        <ul>
          <li>SUM</li>
          <li>AVERAGE</li>
          <li>MIN</li>
          <li>MAX</li>
          <li>COUNT</li>
        </ul><br>
      </li>
      <li>
        <p><strong>Create a Pivot Table:</strong> Use the PivotTable feature to create a pivot table that displays the Department field in the Rows section, and the Equipment Count in the Values section, so that the pivot table displays the sum of equipment count by department.</p>
      </li>
      <li>
        <p><strong>Sort the pivot table data:</strong> Use the Sort By Value setting on the pivot table to sort it in descending order by the sum of equipment count.</p>
      </li>
      <li>
        <p><strong>Make two more pivot tables exactly the same as task 3:</strong> Follow the same steps you performed in Tasks 3 and 4 to create two more identical pivot tables so that you end up with 3 worksheets that contain identical pivot tables.</p>
      </li>
      <li>
        <p><strong>Analyze data in the pivot table:</strong> Use the PivotTable Fields pane to manipulate and analyze data in the two copied pivot table as follows:</p>
        <ul>
          <li>In pivot table 2 add the Equipment Class field below the Department field so that the different vehicle types appear under each department with their respective counts.</li>
          <li>Collapse all fields except the top one - <strong>Transportation</strong></li>
          <li>In pivot table 3 add the Equipment Class field above the Department field so that the different vehicle types appear first, with the different departments listed underneath each vehicle type with their respective counts.</li>
          <li>Collapse all fields except the top one - <strong>CUV</strong></li>
        </ul><br>
      </li>
      <li>
        <p><strong>Save your workbook:</strong> Use 'Save As' to save your workbook as <strong>Montgomery_Fleet_Equipment_Inventory_FA_PART_2_END.XLSX</strong></p>
      </li>
    </ol>
    <h2>Grading Information</h2>
    <p>For your assignment to be graded in a subsequent step in this course, you will be required to upload the completed Excel workbook that you saved in Task 7.</p>
    <p>The <strong>main grading criteria</strong> will be:</p>
    <ul>
      <li>Is the data formatted as a table?</li>
      <li>Are the AutoSum values correct?</li>
      <li>Has the correct pivot table been created and sorted?</li>
      <li>Has the pivot table been created two more times?</li>
      <li>Have the correct fields been used in pivot tables 2 and 3?</li>
      <li>Has the workbook been saved correctly?</li>
    </ul>
    <p>You <strong>will not be judged</strong> on:</p>
    <ul>
      <li>Your English language, including spelling or grammatical mistakes.</li>
      <li>The content of any text or image(s) or where a link is hyperlinked to.</li>
    </ul>
    <h2>Author(s)</h2>
    <ul>
      <li><a href="https://www.linkedin.com/in/stevelryan?utm_medium=Exinfluencer&amp;utm_source=Exinfluencer&amp;utm_content=000026UJ&amp;utm_term=10006555&amp;utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDA0130ENSkillsNetwork20531059-2021-01-01" target="_blank" rel="external">Steve Ryan</a></li>
    </ul>
    <h3>Other Contributor(s)</h3>
    <ul>
      <li><a href="https://www.linkedin.com/in/sandipsahajoy/?utm_medium=Exinfluencer&amp;utm_source=Exinfluencer&amp;utm_content=000026UJ&amp;utm_term=10006555&amp;utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDA0130ENSkillsNetwork20531059-2021-01-01" target="_blank" rel="external">Sandip Saha Joy</a></li>
    </ul>
    <h2>Changelog</h2>
    <table>
      <thead>
        <tr>
          <th>Date</th>
          <th>Version</th>
          <th>Changed by</th>
          <th>Change Description</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>2021-10-11</td>
          <td>1.3</td>
          <td>Malika</td>
          <td>Updated dataset source link</td>
        </tr>
        <tr>
          <td>2020-10-02</td>
          <td>1.2</td>
          <td>Steve Ryan</td>
          <td>Edited to use the most recent version of the Final Assignment instructions</td>
        </tr>
        <tr>
          <td>2020-09-02</td>
          <td>1.1</td>
          <td>Steve Ryan</td>
          <td>Edited to use separate datasets for Parts 1 and 2</td>
        </tr>
        <tr>
          <td>2020-08-24</td>
          <td>1.0</td>
          <td>Steve Ryan</td>
          <td>Post ID review and published in course</td>
        </tr>
        <tr>
          <td>2020-08-23</td>
          <td>0.2</td>
          <td>Sandip Saha Joy</td>
          <td>Converted to markdown in GitLab</td>
        </tr>
        <tr>
          <td>2020-08-22</td>
          <td>0.1</td>
          <td>Steve Ryan</td>
          <td>Initial version created in Word</td>
        </tr>
      </tbody>
    </table>
    <h2></h2>
    <h3 align="center">© IBM Corporation 2020. All rights reserved.</h3>
    <h3></h3>
    <script>window.addEventListener('load', function() {
snFaculty.inject();
});</script>
    <script src="./instructions-2_files/inject.43989f87.js.download"></script>
    <script src="./instructions-2_files/highlight.min.js.download"></script>
    <script src="./instructions-2_files/highlightjs-badge.min.js.download"></script>
  

<style>
@media print {
   .code-badge { display: none; }
}
    .code-badge-pre {
        position: relative;
    }
    .code-badge {
        display: flex;
        flex-direction: row;
        white-space: normal;
        background: transparent;
        background: #333;
        color: white;
        font-size: 0.875em;
        opacity: 0.5;
        transition: opacity linear 0.5s;
        border-radius: 0 0 0 7px;
        padding: 5px 8px 5px 8px;
        position: absolute;
        right: 0;
        top: 0;
    }
    .code-badge.active {
        opacity: 0.8;
    }

    .code-badge:hover {
        opacity: .95;
    }

    .code-badge a,
    .code-badge a:hover {
        text-decoration: none;
    }

    .code-badge-language {
        margin-right: 10px;
        font-weight: 600;
        color: goldenrod;
    }
    .code-badge-copy-icon {
        font-size: 1.2em;
        cursor: pointer;
        padding: 0 7px;
        margin-top:2;
    }
    .fa.text-success:{ color: limegreen !important }
</style><div id="CodeBadgeTemplate" style="display:none">
    <div class="code-badge">
        <div class="code-badge-language">{{language}}</div>
        <div title="Copy to clipboard">
            <i class="{{copyIconClass}} code-badge-copy-icon"></i>
        </div>
     </div>
</div></body></html>