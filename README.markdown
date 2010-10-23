## Description
jQuery Highlighter is a key words highlight plugin for jQuery.  
Online test page: <http://xujinnet.github.com/jQuery-Highlighter/jQuery-Highlighter-Test-Page.html>

## Main Futures
1. Support for multiple keywords.
2. Can overlap between multiple keywords.
3. Can cancel the highlighted keywords.

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
6. If you want to cancel the highlighted keywords or need to highlight keywords several times within the same container tag:

        // Highlight key words.
        // Note the second argument.
        $("#div_Text").highlight(someKeyWords, {needUnhighlight: true});
        
        // Cancel the highlighted keywords.
        $("#div_Text").unhighlight();

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
Specifies whether need the function of cancel the highlighted keywords or highlight keywords several times within the same container tag.  
Data Type: Boolean  
Default Value: false

## License
This plugin is licensed under the CDDL v1.0. You can find the full license text here: http://www.opensource.org/licenses/cddl1.txt.

## Contact Information
E-Mail: XuJin.Net@Gmail.COM  
QQ: 22492791