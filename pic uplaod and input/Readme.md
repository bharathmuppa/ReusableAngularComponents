AdvanceInputFeatures:

steps to use:




    1)Include AdvanceInputFeautures.js after angular and jquery plugin
    2)Inject advanceInputFeatures as dependency in your angular module
        eg:angular.module("myApp",["AdvanceInputFeautures"]);
    3)In input field add input-validation attribute and assign the required pattern as per api for validating input fields as per requirement.
        <input type="text" input-validation="withTwoDigits" ng-model="data" />
        
    4)In input fields add  upload-file attribute for uploading images(videos or files in next version)    
        <input upload-file ng-model="picData">





features available for Validation directive :
  
  
  
  
      input-validation="withTwoDigits" -->for allowing any numbers with two decimal values mostly for money related entries
      input-validation="restrictSpaces"-->for restricting spacess in field
      input-validation="pwdCheck"     -->for field with type="password"
      input-validation="onlyNumbers"  -->for fields that allow only numbers
      input-validation="search"       -->for fields that are of type search
      mxlength="n" -->for allowing less than 'n' chars in fields
      mnlength="n" -->for allowing  minimum of 'n' chars in fields
      
      
fixed issues (Those are most common with Hybrid apps in angular ):
  
  
  
   1)key code issue refer https://code.google.com/p/chromium/issues/detail?id=118639
   2)android back space issue refer http://www.codeitive.com/0iNWVUPjUP/android-native-backspace-is-not-working-on-a-input-field-which-uses-custom-directives-for-validation.html
   3)reduced frozen keyboard on nexus and samsung issues refer https://code.google.com/p/android/issues/detail?id=42518
    4)ng-trim and max length restriction issues in angular
  
  
  
  features available for  uploading images
      
      
      
       picId="divname" -->for placing pic selected from local directory to a particular div
       url="167.54.12.9:8080/..... "  -->storing image base64 code to particular server
       success="successCallBack" -->on hitting data successfully this call back is triggered with some response
       fail="failureCallBack" -->on failure this call back is triggered with some reason for rejection
        
        
        
        
        

