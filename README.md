# Wix-Website-Member-Directory
The following Video is a demo of a Therapist &amp; Supervisor Directory I independently developed for WAMFT and still a work in progress. I’m in charge of the complete development life cycle of the project. 

This was created with JavaScript and the Velo API to meet WAMFT requested requirements for their directory. Its purpose is to allow their member to locate therapist and supervisors in Washington state. 

  Directory Overall Look / Design
  
The colors and styling of the directory were chosen to match the client’s color scheme and look of the rest of their website. 
Mini profiles display snippets of information the client felt were important for users to be aware of during their search. A button labeled “Profile” directs the user to the member’s specific detailed profile. 

Please be aware in the demo that some fields within the mini profile do no contain text while others do. The data represented is test data and made up and blank sections are edge cases to confirm the system can handle undefined member data. 

At top of the directory is results count indicator that allows a user to be informed about the amount of results they have gotten on their search as well as their position and results contained on the page. This can also be found at the bottom accompanied by pagination bar. 

  Filter Design Breakdown

It supports up to 23 different filter options. These are broken into 3 categories. Information that applies to All Members, Supervisor, and Therapist. See below for details: 

1.	Sort By Last Name
  a.	Ascending 
  b.	Descending
  2.	Supervisor
3.	Therapist 
4.	All Members
  a.	Location: County
  b.	Location: City
  c.	Race/Ethnicity
  d.	Sexual Orientation
  e.	Gender Identity/Sex
  f.	Disability Status
  g.	Languages Spoken
  h.	Clinical Focus Areas
  i.	Treatment Techniques
  j.	License Type
  k.	Years as an MFT
  l.	Practice Setting
5.	Supervisor
  a.	Credentials
  b.	Years Supervising
  c.	Supervision Offered
  d.	Online Supervision
6.	Therapist
  a.	Therapy Structure
  b.	Payments Accepted: Insurance
  c.	Payments Accepted: Out of Pocket
  d.	Sliding Scale:
  e.	Insurance Accepted

Element Types

Multiple Filter types were used to meet the client’s request. These are switches, dropdowns, radio groups, checkbox groups, sliders, and a custom element I developed that is a dropdown with checkbox groups inlayed to allow a user to apply multiple types that apply for that given filter group as these contained over 80+ options. 

Filter Processes

The filters will be automatically applied when the user selects a given filter to increase usability for the user, except for the custom element type. This has an apply button built in so that the filters selection can be processed in batch to improve efficiency of the directory. 

Each filter except for the switches at the top are contained within a collapsible container to reduce clutter and so that a user can focus solely on the filters that concern them. The user can click anywhere on the button and does not have to be directly on the collapse or expand icon. This choice was to prompt ease of use.
When a user selects a filter, a tab is created at the top of the directory so the user can easily see what filters are currently applied. The user may also select/click on this tab to easily remove the filter if they wish to.  Additionally, a loading animation is played to mask pop-in so that user does not witness the content of the directory loading in. 

The switches labeled Supervisor and Therapist are unique in the actions that take place when they are activated or deactivated. When are user actives / selects the filter option to filter members by Supervisor it will also expand / add an additional filter block that contains additional filters options that only apply to Supervisors. If the user, then deactivate the switch or clicks the filter tag. It will remove this additional section. This is also the case for the Therapist switch. 
