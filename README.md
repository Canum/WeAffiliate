About WebAffiliate 

 

It Creates a feedback widget that feels like a part of your website's native design 

Dynamic screenshots, categorization of responses and custom fields to enrich your feedback collection. 

That's not all! 

There's a lot more from where the above came from 

Custom Forms 

Define your own feedback categories. Add fields for each category using our drag-drop form builder. 

Custom Styling 

Style the feedback form in your own way. Use our online CSS editor to create a skin for your site. 

Feedback Inbox 

Inbox of support tickets. Filter by categories and workflow status. Manage feedback and replies. 

Instant Modification 

All changes done on project dashboard are reflected real-time. No integration code changes are required. 

 

 

 

npm -i in each folder and run 

pre------ 

      localhost:3000-----Front-end server 

      localhost:5000-----Back-end  Server 

      localhost:9001-----Client Server 

**************************************************************************** 

Go to ClientServer/views/contactForm.ejs and copy this script to your code 

<script async="async" defer="defer" id="feedback_form_tag" type="text/javascript"> 

    var clientIDForForm; 

    (function(i, document,id ){ 

                    i['getClientIDObject'] = id; 

                    i[id] = i[id] || function() { 

                      (i[id].q = i[id].q || []).push(arguments) 

                    }, i[id].l = 1 * new Date(); 

                    //console.log(i[id]); 

                    var f = document.createElement("script"), 

                        d = document.getElementById("feedback_form_tag"); 

                    f.type = "text/javascript", f.async = !0, f.src = "http://localhost:3000/js/form.js", d.parentNode.insertBefore(f, d) 

  })(window, document,'getClientID') 

    setTimeout(function(){ 

        var widgetid=localStorage.getItem('id') 

        getClientID(11);},500); 

******Replace getClientID(11) by getCLientID('your widgetID')************ 

  

******You Can Check your form at 'localhost:3000/clientForm/{yourwidgetID}****** 

  

******At backend Allow Access-Origin to Client Server from 'server.js'******* 

  

  

  

 

 
 

 
