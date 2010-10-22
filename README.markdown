## Description
jQuery Highlighter is a key words highlight plugin for jQuery.

----------

## Quick Start
1. Include jQuery and the Highlighter plugin script file in your HTML page:

        <script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/1.4.3/jquery.min.js"></script>
        <script type="text/javascript" src="jquery.highlighter-1.0.0.min.js"></script>

2. In your HTML body create a container tag pair that will hold some text.Give it an id or class attribute (e.g. "News-Pagination"). This attribute can used as the selector for jQuery.
3. Write some text into the previously created container tag, that contain the key words you want to search .
4. Write the JavaScript code in your HTML head:

        <script type="text/javascript">
            // Some key words that within the previously created container tag.
            // Use one space to separate multiple keywords.
        	var someKeyWords = "......";
        	$("#div_Text").highlight(someKeyWords);
        </script>

5. Use your favorite browser to view this page, you will see the keywords are marked red.
6. If you want to cancel the highlighted keywords:

        // Highlight key words.
        // Note the second argument.
        $("#div_Text").highlight(someKeyWords, {needUnhighlight: true});
        
        // Cancel the highlighted keywords.
        $("#div_Text").unhighlight();

----------

## Available Options
The following list describes what options you have for the second argument of the method "highlight" (option object):

**hClass**  
Specifies the CSS class used to highlight key words.  
Data Type: String  
Default Value: null

**hColor**  
Specifies the color used to highlight key words. If you setted the **hClass** option, this option will be ignored.  
Data Type: String  
Default Value: "#C03"

**separator**  
The symbol used to separate multiple keywords.  
Data Type: String  
Default Value: " "

**wrapper**  
Specifies the HTML tag used to wrap the keywords.  
Data Type: String  
Default Value: "em"

**useDefaultStyle**  
When not set hClass option, specify whether to use the default style to highlight the keywords (eg: use the **hColor** option).  
Data Type: Boolean  
Default Value: true

**needUnhighlight**  
Specifies whether need the function of cancel the highlighted keywords.  
Data Type: Boolean  
Default Value: false