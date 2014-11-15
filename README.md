JavaToast Library for Java Desktop Program
========================================
----------------------------------------

1) How to use JavaToast
=======================
    
        1. First you must have to import "JavaToast.jar" in the project library folder
        2. set API where you want to show Toast message.
        
2) How to set API
=================
    
        1. set API by calling the "new JToast().makeToast(Some args)" method.
        
3) API discription
==================
    
        There are two override method in the JToast class
        -------------------------------------------------
        
           1. makeToast( JFrame frame, String message, int timeOfSecond)
           2. makeToast( JFrame frame, String message, int timeOfSecond, int messageType)
           
4) Example
==========
    
        1. If you only want to show text message , you can add below API
            
            "new JToast().makeToast( JFrame frame, String message, int timeOfSecond);"
            discription of args
            -------------------
            
                frame= JFrame, where you want to show message.you can set value "this" to show in current JFrame
                message= the text what you want to show
                timeOfSecond= how many time you want to show message (in second format)
                
                final API= "new JToast().makeToast( this, "I am a Toast Message without icon", 3);"
                demo = https://dl.dropboxusercontent.com/s/ftdain4yecs6uws/Capture.PNG?dl=0
                
        
        2. If you want to show text message with icon , you can add below API
            
            "new JToast().makeToast( JFrame frame, String message, int timeOfSecond, int type);"
            discription of args
            -------------------
            
                frame= JFrame, where you want to show message.you can set value "this" to show in current JFrame
                message= the text what you want to show
                timeOfSecond= how many time you want to show message (in second format)
                type= type of icon
                
                    Icon type
                    ---------
                       1) JToast.type_of_succes
                       2) JToast.type_of_ok
                       3) JToast.type_of_notification
                       4) JToast.type_of_error
                       5) JToast.type_of_info
                
                final API= "new JToast().makeToast(this, "I am a Toast Message with icon", 3, JToast.type_of_succes);"
                demo = https://dl.dropboxusercontent.com/s/whpzsoyafczsbqa/Capture2.PNG?dl=0
                
