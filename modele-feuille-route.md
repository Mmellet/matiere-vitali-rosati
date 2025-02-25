 <!DOCTYPE html>
<html lang="fr-FR">
    <head>
        <meta http-equiv="X-UA-Compatible" content="IE=edge"/>
        <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=1"/>
        <meta http-equiv="content-type" content="text/html;charset=UTF-8" />
        <meta http-equiv="cache-control" content="no-cache,no-store"/>
        <meta http-equiv="pragma" content="no-cache"/>
        <meta http-equiv="expires" content="-1"/>
        <meta name='mswebdialog-title' content='Connecting to Universit&#233; de Sherbrooke'/>

        <title>Connexion</title>
        <script type='text/javascript'>
//<![CDATA[
function LoginErrors(){this.userNameFormatError = 'Entrez votre ID d\u0026#39;utilisateur au format \u0026#171; domaine\\utilisateur \u0026#187; ou \u0026#171; utilisateur@domaine \u0026#187;.'; this.passwordEmpty = 'Entrez votre mot de passe.'; this.passwordTooLong = 'Le mot de passe est trop long (\u0026gt; 128 caract\u0026#232;res).';}; var maxPasswordLength = 128;
//]]>
</script>

<script type='text/javascript'>
//<![CDATA[
// Copyright (c) Microsoft Corporation.  All rights reserved.
function InputUtil(errTextElementID, errDisplayElementID) {

    if (!errTextElementID)  errTextElementID = 'errorText'; 
    if (!errDisplayElementID)  errDisplayElementID = 'error'; 

    this.hasFocus = false;
    this.errLabel = document.getElementById(errTextElementID);
    this.errDisplay = document.getElementById(errDisplayElementID);
};
InputUtil.prototype.canDisplayError = function () {
    return this.errLabel && this.errDisplay;
}
InputUtil.prototype.checkError = function () {
    if (!this.canDisplayError){
        throw new Error ('Error element not present');
    }
    if (this.errLabel && this.errLabel.innerHTML) {
        this.errDisplay.style.display = '';        
        var cause = this.errLabel.getAttribute('for');
        if (cause) {
            var causeNode = document.getElementById(cause);
            if (causeNode && causeNode.value) {
                causeNode.focus();
                this.hasFocus = true;
            }
        }
    }
    else {
        this.errDisplay.style.display = 'none';
    }
};
InputUtil.prototype.setInitialFocus = function (input) {
    if (this.hasFocus) return;
    var node = document.getElementById(input);
    if (node) {
        if ((/^\s*$/).test(node.value)) {
            node.focus();
            this.hasFocus = true;
        }
    }
};
InputUtil.prototype.setError = function (input, errorMsg) {
    if (!this.canDisplayError) {
        throw new Error('Error element not present');
    }
    input.focus();

    if (errorMsg) {
        this.errLabel.innerHTML = errorMsg;
    }
    this.errLabel.setAttribute('for', input.id);
    this.errDisplay.style.display = '';
};
InputUtil.makePlaceholder = function (input) {
    var ua = navigator.userAgent;

    if (ua != null && 
        (ua.match(/MSIE 9.0/) != null || 
         ua.match(/MSIE 8.0/) != null ||
         ua.match(/MSIE 7.0/) != null)) {
        var node = document.getElementById(input);
        if (node) {
            var placeholder = node.getAttribute("placeholder");
            if (placeholder != null && placeholder != '') {
                var label = document.createElement('input');
                label.type = "text";
                label.value = placeholder;
                label.readOnly = true;
                label.style.position = 'absolute';
                label.style.borderColor = 'transparent';
                label.className = node.className + ' hint';
                label.tabIndex = -1;
                label.onfocus = function () { this.nextSibling.focus(); };

                node.style.position = 'relative';
                node.parentNode.style.position = 'relative';
                node.parentNode.insertBefore(label, node);
                node.onkeyup = function () { InputUtil.showHint(this); };
                node.onblur = function () { InputUtil.showHint(this); };
                node.style.background = 'transparent';

                node.setAttribute("placeholder", "");
                InputUtil.showHint(node);
            }
        }
    }
};
InputUtil.focus = function (inputField) {
    var node = document.getElementById(inputField);
    if (node) node.focus();
};
InputUtil.hasClass = function(node, clsName) {
    return node.className.match(new RegExp('(\\s|^)' + clsName + '(\\s|$)'));
};
InputUtil.addClass = function(node, clsName) {
    if (!this.hasClass(node, clsName)) node.className += " " + clsName;
};
InputUtil.removeClass = function(node, clsName) {
    if (this.hasClass(node, clsName)) {
        var reg = new RegExp('(\\s|^)' + clsName + '(\\s|$)');
        node.className = node.className.replace(reg, ' ');
    }
};
InputUtil.showHint = function (node, gotFocus) {
    if (node.value && node.value != '') {
        node.previousSibling.style.display = 'none';
    }
    else {
        node.previousSibling.style.display = '';
    }
};
InputUtil.updatePlaceholder = function (input, placeholderText) {
    var node = document.getElementById(input);
    if (node) {
        var ua = navigator.userAgent;
        if (ua != null &&
            (ua.match(/MSIE 9.0/) != null ||
            ua.match(/MSIE 8.0/) != null ||
            ua.match(/MSIE 7.0/) != null)) {
            var label = node.previousSibling;
            if (label != null) {
                label.value = placeholderText;
            }
        }
        else {
            node.placeholder = placeholderText;
        }
    }
};

//]]>
</script>


        
        <link rel="stylesheet" type="text/css" href="/adfs/portal/css/style.css?id=07B8CFB17C4ADBD235B4A76F602C3C657699ADF12BD5E990C71D12703DB69DC1" /><style>.illustrationClass {background-image:url(/adfs/portal/illustration/illustration.jpg?id=BD5AF2CCCD0B345890EC9D9F17E1C8718ADECDDC78D30B23D72F107858E67B75);}</style>

    </head>
    <body dir="ltr" class="body">
    <div id="noScript" style="position:static; width:100%; height:100%; z-index:100">
        <h1>JavaScript requis</h1>
        <p>JavaScript est requis. Ce navigateur Web ne prend pas en charge JavaScript ou JavaScript n&#39;est pas activ&#233; dans ce navigateur Web.</p>
        <p>Consultez l&#39;aide de votre navigateur Web pour savoir si votre navigateur Web prend en charge JavaScript ou pour activer JavaScript.</p>
    </div>
    <script type="text/javascript" language="JavaScript">
         document.getElementById("noScript").style.display = "none";
    </script>
    <div id="fullPage">
        <div id="brandingWrapper" class="float">
            <div id="branding"></div>
        </div>
        <div id="contentWrapper" class="float">
            <div id="content">
                <div id="header">
                    <img class='logoImage' id='companyLogo' src='/adfs/portal/logo/logo.png?id=9E876FE5C9052B42115B1C856D49BA499305C133A81028CEEDEE79856EBC7573' alt='Universit&#233; de Sherbrooke'/>
                </div>
                <main>
                    <div id="workArea">
                        
    <div id="authArea" class="groupMargin">
        
        
        
    <div id="loginArea">        
        <div id="loginMessage" class="groupMargin">Se connecter</div>

        <form method="post" id="loginForm" autocomplete="off" novalidate="novalidate" onKeyPress="if (event && event.keyCode == 13) Login.submitLoginRequest();" action="/adfs/ls/?SAMLRequest=lVJbT8IwFP4rS9%2B3bjMMbIAEIUYSVCLogy%2Fm0J5J49bOns7Lv7cMjRgviUkfmnPOdzlfOySoq0ZMWr81V%2FjYIvnopa4Mia4xYq0zwgJpEgZqJOGlWE3OFyJPUtE46620FTuA%2FI0AInReW8Oi%2BWzE7opSSswgVyg3WQaDAo8HqiwGCvtHWYFlAaDSfpH2FYtu0FFAjlggCnCiFueGPBgfSmnei9M8znvrNBNZOMUti2ZhG23Ad6it9w0JziGsisbrUsuuk7S0Rbdx1j5gIoGDKolXxFk0%2BTA7tYbaGt0K3ZOWeH21%2BKSrrVUVfiMJInwXR86p2V9ikJQ02%2BZnBIuW72GeaKO0uf87x81%2BiMTZer2Ml5erNRsPdzKiy8WN%2F2OvRg8KPOzcDfkhy3D%2FOy6C%2Fny2tJWWr9GpdTX43%2B1lSdZVtIrLblS0hhqUIXAMrzipKvs8dQgeR8y7Fhkf70W%2F%2FsLxGw%3D%3D&RelayState=https%3A%2F%2Fmoodle.usherbrooke.ca%2Fpluginfile.php%2F4590695%2Fmod_label%2Fintro%2Fmodele-feuille-route.md&SigAlg=http%3A%2F%2Fwww.w3.org%2F2001%2F04%2Fxmldsig-more%23rsa-sha256&Signature=Z%2BV1ilz5Hk9k%2BDIX38YuXAg8OTsBQ67U1%2FyAdubAqgdP8Abhc8wAigdDUzo0oWaBbu2EIJ8vAF2sXbmoxtHy6gVF2SOCloWywLbfzcx52L9NSLYjCQPXAUeqBkqalxQoT%2F0YG4VcqRpbDKo87a%2BJ%2BcerbOab6aY%2FoiimGtPBizJG1GY4OwrifqH1o8sFhXR6d%2BHpPz3GbVm9lXV3fFY%2BELs%2FKvHZ76YiRBYYfyqNzeSqcYyqiqErdxP2x4y5rRYjJybMJvtp8UKWLiwwyxGKZocnUU9xP5wJ2Qxf9E7NJXLmK2zNkL%2BEfmp%2BeCFgKv%2BYtTbLlhvVTOKGyWbqgOi7HQ%3D%3D&client-request-id=5c941109-3c35-428d-b672-0080010000d5" >
            <div id="error" class="fieldMargin error smallText">
                <span id="errorText" for="" aria-live="assertive" role="alert"></span>
            </div>

            <div id="formsAuthenticationArea">
                <div id="userNameArea">
                    <label id="userNameInputLabel" for="userNameInput" class="hidden">Compte d&#39;utilisateur</label>
                    <input id="userNameInput" name="UserName" type="email" value="" tabindex="1" class="text fullWidth"
                        spellcheck="false" placeholder="xyz@example.com" autocomplete="off"/>
                </div>

                <div id="passwordArea">
                    <label id="passwordInputLabel" for="passwordInput" class="hidden">Mot de passe</label>
                    <input id="passwordInput" name="Password" type="password" tabindex="2" class="text fullWidth"
                        placeholder="Mot de passe" autocomplete="off"/>
                </div>
                <div id="kmsiArea" style="display:''">
                    <input type="checkbox" name="Kmsi" id="kmsiInput" value="true" tabindex="3" />
                    <label for="kmsiInput">Maintenir la connexion</label>
                </div>
                <div id="submissionArea" class="submitMargin">
                    <span id="submitButton" class="submit" tabindex="4" role="button"
                        onKeyPress="if (event && event.keyCode == 32) Login.submitLoginRequest();"
                        onclick="return Login.submitLoginRequest();">Connexion</span>
                </div>
            </div>
            <input id="optionForms" type="hidden" name="AuthMethod" value="FormsAuthentication"/>
        </form>

             <div id="authOptions">
         <form id="options" method="post" action="https://authentification.usherbrooke.ca:443/adfs/ls/?SAMLRequest=lVJbT8IwFP4rS9%2B3bjMMbIAEIUYSVCLogy%2Fm0J5J49bOns7Lv7cMjRgviUkfmnPOdzlfOySoq0ZMWr81V%2FjYIvnopa4Mia4xYq0zwgJpEgZqJOGlWE3OFyJPUtE46620FTuA%2FI0AInReW8Oi%2BWzE7opSSswgVyg3WQaDAo8HqiwGCvtHWYFlAaDSfpH2FYtu0FFAjlggCnCiFueGPBgfSmnei9M8znvrNBNZOMUti2ZhG23Ad6it9w0JziGsisbrUsuuk7S0Rbdx1j5gIoGDKolXxFk0%2BTA7tYbaGt0K3ZOWeH21%2BKSrrVUVfiMJInwXR86p2V9ikJQ02%2BZnBIuW72GeaKO0uf87x81%2BiMTZer2Ml5erNRsPdzKiy8WN%2F2OvRg8KPOzcDfkhy3D%2FOy6C%2Fny2tJWWr9GpdTX43%2B1lSdZVtIrLblS0hhqUIXAMrzipKvs8dQgeR8y7Fhkf70W%2F%2FsLxGw%3D%3D&RelayState=https%3A%2F%2Fmoodle.usherbrooke.ca%2Fpluginfile.php%2F4590695%2Fmod_label%2Fintro%2Fmodele-feuille-route.md&SigAlg=http%3A%2F%2Fwww.w3.org%2F2001%2F04%2Fxmldsig-more%23rsa-sha256&Signature=Z%2BV1ilz5Hk9k%2BDIX38YuXAg8OTsBQ67U1%2FyAdubAqgdP8Abhc8wAigdDUzo0oWaBbu2EIJ8vAF2sXbmoxtHy6gVF2SOCloWywLbfzcx52L9NSLYjCQPXAUeqBkqalxQoT%2F0YG4VcqRpbDKo87a%2BJ%2BcerbOab6aY%2FoiimGtPBizJG1GY4OwrifqH1o8sFhXR6d%2BHpPz3GbVm9lXV3fFY%2BELs%2FKvHZ76YiRBYYfyqNzeSqcYyqiqErdxP2x4y5rRYjJybMJvtp8UKWLiwwyxGKZocnUU9xP5wJ2Qxf9E7NJXLmK2zNkL%2BEfmp%2BeCFgKv%2BYtTbLlhvVTOKGyWbqgOi7HQ%3D%3D&client-request-id=5c941109-3c35-428d-b672-0080010000d5">
             <script type="text/javascript">
                function SelectOption(option) {
                    var w = document.getElementById('waitingWheelDiv');
                    if(w) w.style.display = 'inline';
                    var i = document.getElementById('optionSelection');
                    i.value = option;
                    document.forms['options'].submit();
                    return false;
                }
             </script>
             <input id="optionSelection" type="hidden" name="AuthMethod" />
             <input id="userNameInputOptionsHolder" name="UserName" value="" type="hidden"/>
             <div id='authOptionLinks' class='groupMargin'><div id="waitingWheelDiv" style="display: none;"><div id="WaitingWheel">
    <!-- NOTE: This style portion is identical to cookie pull page, they are not in shared css file because of legacy dependancies for custom themes-->
    <!-- CSS for small "waiting" wheel -->
    <style>
        #floatingCirclesG {
            position: relative;
            width: 125px;
            height: 125px;
            margin: auto;
            transform: scale(0.4);
            -o-transform: scale(0.4);
            -ms-transform: scale(0.4);
            -webkit-transform: scale(0.4);
            -moz-transform: scale(0.4);
        }

        .f_circleG {
            position: absolute;
            height: 22px;
            width: 22px;
            border-radius: 12px;
            -o-border-radius: 12px;
            -ms-border-radius: 12px;
            -webkit-border-radius: 12px;
            -moz-border-radius: 12px;
            animation-name: f_fadeG;
            -o-animation-name: f_fadeG;
            -ms-animation-name: f_fadeG;
            -webkit-animation-name: f_fadeG;
            -moz-animation-name: f_fadeG;
            animation-duration: 1.2s;
            -o-animation-duration: 1.2s;
            -ms-animation-duration: 1.2s;
            -webkit-animation-duration: 1.2s;
            -moz-animation-duration: 1.2s;
            animation-iteration-count: infinite;
            -o-animation-iteration-count: infinite;
            -ms-animation-iteration-count: infinite;
            -webkit-animation-iteration-count: infinite;
            -moz-animation-iteration-count: infinite;
            animation-direction: normal;
            -o-animation-direction: normal;
            -ms-animation-direction: normal;
            -webkit-animation-direction: normal;
            -moz-animation-direction: normal;
        }

        #frotateG_01 {
            left: 0;
            top: 51px;
            animation-delay: 0.45s;
            -o-animation-delay: 0.45s;
            -ms-animation-delay: 0.45s;
            -webkit-animation-delay: 0.45s;
            -moz-animation-delay: 0.45s;
        }

        #frotateG_02 {
            left: 15px;
            top: 15px;
            animation-delay: 0.6s;
            -o-animation-delay: 0.6s;
            -ms-animation-delay: 0.6s;
            -webkit-animation-delay: 0.6s;
            -moz-animation-delay: 0.6s;
        }

        #frotateG_03 {
            left: 51px;
            top: 0;
            animation-delay: 0.75s;
            -o-animation-delay: 0.75s;
            -ms-animation-delay: 0.75s;
            -webkit-animation-delay: 0.75s;
            -moz-animation-delay: 0.75s;
        }

        #frotateG_04 {
            right: 15px;
            top: 15px;
            animation-delay: 0.9s;
            -o-animation-delay: 0.9s;
            -ms-animation-delay: 0.9s;
            -webkit-animation-delay: 0.9s;
            -moz-animation-delay: 0.9s;
        }

        #frotateG_05 {
            right: 0;
            top: 51px;
            animation-delay: 1.05s;
            -o-animation-delay: 1.05s;
            -ms-animation-delay: 1.05s;
            -webkit-animation-delay: 1.05s;
            -moz-animation-delay: 1.05s;
        }

        #frotateG_06 {
            right: 15px;
            bottom: 15px;
            animation-delay: 1.2s;
            -o-animation-delay: 1.2s;
            -ms-animation-delay: 1.2s;
            -webkit-animation-delay: 1.2s;
            -moz-animation-delay: 1.2s;
        }

        #frotateG_07 {
            left: 51px;
            bottom: 0;
            animation-delay: 1.35s;
            -o-animation-delay: 1.35s;
            -ms-animation-delay: 1.35s;
            -webkit-animation-delay: 1.35s;
            -moz-animation-delay: 1.35s;
        }

        #frotateG_08 {
            left: 15px;
            bottom: 15px;
            animation-delay: 1.5s;
            -o-animation-delay: 1.5s;
            -ms-animation-delay: 1.5s;
            -webkit-animation-delay: 1.5s;
            -moz-animation-delay: 1.5s;
        }

        @keyframes f_fadeG {
            0% {
                background-color: rgb(47, 146, 212);
            }

            100% {
                background-color: rgb(255, 255, 255);
            }
        }

        @-o-keyframes f_fadeG {
            0% {
                background-color: rgb(47, 146, 212);
            }

            100% {
                background-color: rgb(255, 255, 255);
            }
        }

        @-ms-keyframes f_fadeG {
            0% {
                background-color: rgb(47, 146, 212);
            }

            100% {
                background-color: rgb(255, 255, 255);
            }
        }

        @-webkit-keyframes f_fadeG {
            0% {
                background-color: rgb(47, 146, 212);
            }

            100% {
                background-color: rgb(255, 255, 255);
            }
        }

        @-moz-keyframes f_fadeG {
            0% {
                background-color: rgb(47, 146, 212);
            }

            100% {
                background-color: rgb(255, 255, 255);
            }
        }
    </style>

    <!-- Div containing small "waiting" wheel -->
    <div id="floatingCirclesG">
        <div class="f_circleG" id="frotateG_01"></div>
        <div class="f_circleG" id="frotateG_02"></div>
        <div class="f_circleG" id="frotateG_03"></div>
        <div class="f_circleG" id="frotateG_04"></div>
        <div class="f_circleG" id="frotateG_05"></div>
        <div class="f_circleG" id="frotateG_06"></div>
        <div class="f_circleG" id="frotateG_07"></div>
        <div class="f_circleG" id="frotateG_08"></div>
    </div>
</div></div></div>
         </form>
      </div>

        <div id="introduction" class="groupMargin">
            <p><a href='https://www.usherbrooke.ca/monacces/mot-de-passe-oubli' target='_blank'>Mot de passe oubli&eacute;?</a></p><div style='margin-top: 2em;'><p class='title'>Avertissement de s&eacute;curit&eacute;<p><p style='margin-bottom: 1rem;'>En utilisant les actifs informationnels mis à votre disposition par l'Universit&eacute; à des fins personnelles ou professionnelles, vous vous engagez à respecter la <a href='https://www.usherbrooke.ca/decouvrir/fileadmin/sites/decouvrir/documents/direction/politiques/2500-036.pdf' target='_blank'>Politique de s&eacute;curit&eacute; de l’information (2500-036)</a> ainsi que la <a href='https://www.usherbrooke.ca/decouvrir/fileadmin/sites/decouvrir/documents/direction/directives/2600-063.pdf' target='_blank'>Directive relative à l’utilisation, à la gestion et à la s&eacute;curit&eacute; des actifs informationnels (2600-063)</a>.</p><p style='margin-bottom: 1rem;'>Pour vous aider à prot&eacute;ger les actifs informationnels de l'Universit&eacute;, consultez le site Web <a href='https://www.usherbrooke.ca/securite-info/politique-et-directive' target='_blank'>S&eacute;curit&eacute; de l’information</a>.</p></div>                     
        </div>

        <script type="text/javascript">
        //<![CDATA[

            function Login() {
            }

            Login.userNameInput = 'userNameInput';
            Login.passwordInput = 'passwordInput';

            Login.initialize = function () {

                var u = new InputUtil();

                u.checkError();
                u.setInitialFocus(Login.userNameInput);
                u.setInitialFocus(Login.passwordInput);
            }();

            Login.submitLoginRequest = function () { 
                var u = new InputUtil();
                var e = new LoginErrors();

                var userName = document.getElementById(Login.userNameInput);
                var password = document.getElementById(Login.passwordInput);

                if (!userName.value || !userName.value.match('[@\\\\]')) {
                    u.setError(userName, e.userNameFormatError);
                    return false;
                }

                if (!password.value) {
                    u.setError(password, e.passwordEmpty);
                    return false;
                }

                if (password.value.length > maxPasswordLength) {
                    u.setError(password, e.passwordTooLong);
                    return false;
                }

                document.forms['loginForm'].submit();
                return false;
            };

            InputUtil.makePlaceholder(Login.userNameInput);
            InputUtil.makePlaceholder(Login.passwordInput);
        //]]>
        </script>
    </div>

    </div>

                    </div>
                </main>
                <div id="footerPlaceholder"></div>
            </div>
            <footer id="footer">
                <div id="footerLinks" class="floatReverse">
                    <div><span id="copyright">&#169; 2018 Microsoft</span><a id="home" class="pageLink footerLink " href="https://www.usherbrooke.ca">Universit&#233; de Sherbrooke</a><a id="helpDesk" class="pageLink footerLink" href="https://www.usherbrooke.ca/decouvrir/nous-contacter/">Contactez-nous</a></div>
                </div>
            </footer>
        </div>     
    </div>
    <script type='text/javascript'>
//<![CDATA[
// Copyright (c) Microsoft Corporation.  All rights reserved.

// This file contains several workarounds on inconsistent browser behaviors that administrators may customize.
"use strict";

//Customize MFA exception
//Begin
var domain_hint = "usherbrooke.ca";
var browserLanguage = navigator.language;
var mfaSecondFactorErr = (browserLanguage === "fr-CA") ? "La méthode d'authentification sélectionnée n'est pas disponible" : "The selected authentication method is not available for";
var mfaProofupMessage = (browserLanguage === "fr-CA") ? "Le service auquel vous voulez vous connecter requiert l'activation de l'authentification à deux facteurs pour votre compte USherbrooke.<br><br>Vous serez redirigé automatiquement dans 30 secondes vers l'interface qui vous permettra de configurer vos options pour la deuxième authentification. Une fois que vous aurez terminé la configuration, veuillez retourner à l'application que vous vouliez accéder. <br><br>Si vous n'êtes pas redirigé automatiquement, veuillez cliquer <a href='{0}'>ici</a>.<br><br>Pour plus de détails sur l'authentification à deux facteurs&nbsp;:<a href='https://www.usherbrooke.ca/services-informatiques/repertoire/acces/authentification-2-facteurs'>https://www.usherbrooke.ca/services-informatiques/repertoire/acces/authentification-2-facteurs</a>" : "The service you want to connect requires two-factor authentication to be enabled for your USherbrooke account.<br><br>You will be automatically redirected in 30 seconds to set up your account for additional security verification. Once you have completed the setup, please return to the application you are attempting to access.<br><br>If you are not redirected automatically, please click <a href='{0}'>here</a>.<br><br>For more information&nbsp;:<a href='https://www.usherbrooke.ca/services-informatiques/repertoire/acces/authentification-2-facteurs'>https://www.usherbrooke.ca/services-informatiques/repertoire/acces/authentification-2-facteurs</a>"
var authArea = document.getElementById("authArea");
if (authArea) {
    var errorMessage = document.getElementById("errorMessage");
    if (errorMessage) {
        if (errorMessage.innerHTML.indexOf(mfaSecondFactorErr) >= 0) {

            //Hide the error message
            var openingMessage = document.getElementById("openingMessage");
            if (openingMessage) {
                openingMessage.style.display = 'none'
            }
            var errorDetailsLink = document.getElementById("errorDetailsLink");
            if (errorDetailsLink) {
                errorDetailsLink.style.display = 'none'
            }

            //Provide a message and redirect to Azure AD MFA Registration Url
            var mfaRegisterUrl = "https://account.activedirectory.windowsazure.com/proofup.aspx?proofup=1&whr=" + domain_hint;
            errorMessage.innerHTML = "<br>" + mfaProofupMessage.replace("{0}", mfaRegisterUrl);
            window.setTimeout(function () { window.location.href = mfaRegisterUrl; }, 30000);
        }
    }
}
//End Customize MFA Exception

// iPhone email friendly keyboard does not include "\" key, use regular keyboard instead.
// Note change input type does not work on all versions of all browsers.
if (navigator.userAgent.match(/iPhone/i) != null) {
    var emails = document.querySelectorAll("input[type='email']");
    if (emails) {
        for (var i = 0; i < emails.length; i++) {
            emails[i].type = 'text';
        }
    }
}

// In the CSS file we set the ms-viewport to be consistent with the device dimensions,
// which is necessary for correct functionality of immersive IE.
// However, for Windows 8 phone we need to reset the ms-viewport's dimension to its original
// values (auto), otherwise the viewport dimensions will be wrong for Windows 8 phone.
// Windows 8 phone has agent string 'IEMobile 10.0'
if (navigator.userAgent.match(/IEMobile\/10\.0/)) {
    var msViewportStyle = document.createElement("style");
    msViewportStyle.appendChild(
        document.createTextNode(
            "@-ms-viewport{width:auto!important}"
        )
    );
    msViewportStyle.appendChild(
        document.createTextNode(
            "@-ms-viewport{height:auto!important}"
        )
    );
    document.getElementsByTagName("head")[0].appendChild(msViewportStyle);
}

// If the innerWidth is defined, use it as the viewport width.
if (window.innerWidth && window.outerWidth && window.innerWidth !== window.outerWidth) {
    var viewport = document.querySelector("meta[name=viewport]");
    viewport.setAttribute('content', 'width=' + window.innerWidth + ', initial-scale=1.0, user-scalable=1');
}

// Gets the current style of a specific property for a specific element.
function getStyle(element, styleProp) {
    var propStyle = null;

    if (element && element.currentStyle) {
        propStyle = element.currentStyle[styleProp];
    }
    else if (element && window.getComputedStyle) {
        propStyle = document.defaultView.getComputedStyle(element, null).getPropertyValue(styleProp);
    }

    return propStyle;
}

// The script below is used for downloading the illustration image
// only when the branding is displaying. This script work together
// with the code in PageBase.cs that sets the html inline style
// containing the class 'illustrationClass' with the background image.
var computeLoadIllustration = function () {
    var branding = document.getElementById("branding");
    var brandingDisplay = getStyle(branding, "display");
    var brandingWrapperDisplay = getStyle(document.getElementById("brandingWrapper"), "display");

    if (brandingDisplay && brandingDisplay !== "none" &&
        brandingWrapperDisplay && brandingWrapperDisplay !== "none") {
        var newClass = "illustrationClass";

        if (branding.classList && branding.classList.add) {
            branding.classList.add(newClass);
        } else if (branding.className !== undefined) {
            branding.className += " " + newClass;
        }
        if (window.removeEventListener) {
            window.removeEventListener('load', computeLoadIllustration, false);
            window.removeEventListener('resize', computeLoadIllustration, false);
        }
        else if (window.detachEvent) {
            window.detachEvent('onload', computeLoadIllustration);
            window.detachEvent('onresize', computeLoadIllustration);
        }
    }
};

if (window.addEventListener) {
    window.addEventListener('resize', computeLoadIllustration, false);
    window.addEventListener('load', computeLoadIllustration, false);
}
else if (window.attachEvent) {
    window.attachEvent('onresize', computeLoadIllustration);
    window.attachEvent('onload', computeLoadIllustration);
}


!function(e,t){"object"==typeof exports&&"undefined"!=typeof module?t():"function"==typeof define&&define.amd?define(t):t()}(0,function(){"use strict";function e(e){var t=this.constructor;return this.then(function(n){return t.resolve(e()).then(function(){return n})},function(n){return t.resolve(e()).then(function(){return t.reject(n)})})}function t(e){return new this(function(t,n){function o(e,n){if(n&&("object"==typeof n||"function"==typeof n)){var f=n.then;if("function"==typeof f)return void f.call(n,function(t){o(e,t)},function(n){r[e]={status:"rejected",reason:n},0==--i&&t(r)})}r[e]={status:"fulfilled",value:n},0==--i&&t(r)}if(!e||"undefined"==typeof e.length)return n(new TypeError(typeof e+" "+e+" is not iterable(cannot read property Symbol(Symbol.iterator))"));var r=Array.prototype.slice.call(e);if(0===r.length)return t([]);for(var i=r.length,f=0;r.length>f;f++)o(f,r[f])})}function n(e){return!(!e||"undefined"==typeof e.length)}function o(){}function r(e){if(!(this instanceof r))throw new TypeError("Promises must be constructed via new");if("function"!=typeof e)throw new TypeError("not a function");this._state=0,this._handled=!1,this._value=undefined,this._deferreds=[],l(e,this)}function i(e,t){for(;3===e._state;)e=e._value;0!==e._state?(e._handled=!0,r._immediateFn(function(){var n=1===e._state?t.onFulfilled:t.onRejected;if(null!==n){var o;try{o=n(e._value)}catch(r){return void u(t.promise,r)}f(t.promise,o)}else(1===e._state?f:u)(t.promise,e._value)})):e._deferreds.push(t)}function f(e,t){try{if(t===e)throw new TypeError("A promise cannot be resolved with itself.");if(t&&("object"==typeof t||"function"==typeof t)){var n=t.then;if(t instanceof r)return e._state=3,e._value=t,void c(e);if("function"==typeof n)return void l(function(e,t){return function(){e.apply(t,arguments)}}(n,t),e)}e._state=1,e._value=t,c(e)}catch(o){u(e,o)}}function u(e,t){e._state=2,e._value=t,c(e)}function c(e){2===e._state&&0===e._deferreds.length&&r._immediateFn(function(){e._handled||r._unhandledRejectionFn(e._value)});for(var t=0,n=e._deferreds.length;n>t;t++)i(e,e._deferreds[t]);e._deferreds=null}function l(e,t){var n=!1;try{e(function(e){n||(n=!0,f(t,e))},function(e){n||(n=!0,u(t,e))})}catch(o){if(n)return;n=!0,u(t,o)}}var a=setTimeout;r.prototype["catch"]=function(e){return this.then(null,e)},r.prototype.then=function(e,t){var n=new this.constructor(o);return i(this,new function(e,t,n){this.onFulfilled="function"==typeof e?e:null,this.onRejected="function"==typeof t?t:null,this.promise=n}(e,t,n)),n},r.prototype["finally"]=e,r.all=function(e){return new r(function(t,o){function r(e,n){try{if(n&&("object"==typeof n||"function"==typeof n)){var u=n.then;if("function"==typeof u)return void u.call(n,function(t){r(e,t)},o)}i[e]=n,0==--f&&t(i)}catch(c){o(c)}}if(!n(e))return o(new TypeError("Promise.all accepts an array"));var i=Array.prototype.slice.call(e);if(0===i.length)return t([]);for(var f=i.length,u=0;i.length>u;u++)r(u,i[u])})},r.allSettled=t,r.resolve=function(e){return e&&"object"==typeof e&&e.constructor===r?e:new r(function(t){t(e)})},r.reject=function(e){return new r(function(t,n){n(e)})},r.race=function(e){return new r(function(t,o){if(!n(e))return o(new TypeError("Promise.race accepts an array"));for(var i=0,f=e.length;f>i;i++)r.resolve(e[i]).then(t,o)})},r._immediateFn="function"==typeof setImmediate&&function(e){setImmediate(e)}||function(e){a(e,0)},r._unhandledRejectionFn=function(e){void 0!==console&&console&&console.warn("Possible Unhandled Promise Rejection:",e)};var s=function(){if("undefined"!=typeof self)return self;if("undefined"!=typeof window)return window;if("undefined"!=typeof global)return global;throw Error("unable to locate global object")}();"function"!=typeof s.Promise?s.Promise=r:s.Promise.prototype["finally"]?s.Promise.allSettled||(s.Promise.allSettled=t):s.Promise.prototype["finally"]=e});


(function () {
    if (Login === undefined) {
        console.error(
            "Could not execute script because the current page is not a " +
            "login page or other scripts were not loaded properly.  " +
            "Undefined object reference is `Login`.");

        return;
    }

    /**
     * Appends organisation domain to username if the username does not already
     * match an email address.  Otherwise, nothing is changed.
     * @returns {boolean} {@code true} if the username is changed, {@code false}
     * otherwise.
     */
    var appendDomainToUsername = function () {
        var lowerUserName = userNameInput.value.toLowerCase().trim();

        if (lowerUserName === '') {
            return false;
        }

        //Check to see if they already included the UPN
        var li = lowerUserName.lastIndexOf('@usherbrooke.ca');
        var la = lowerUserName.lastIndexOf('@');

        if (li === -1 && la === -1) {
            userNameInput.value = userNameInput.value.trim() + '@usherbrooke.ca';
            console.log("append domain @usherbrooke.ca to username [" + userNameInput.value + "]");
            return true;
        }

        return false;
    };

    /**
     * Fetches the user principal name based on the login's username input
     * field.
     *
     * A call to a dedicated web api that takes the alternate username is made
     * to obtain the user principal name associated with it.
     *
     * @returns {Promise<boolean>} {@code true} if the user principal name was found,
     * {@code false} otherwise.
     */
    var identity = function () {
        return new Promise(function (resolve, reject) {
            if (userNameInput.value.trim() === '') {
                return resolve(false);
            }

            var request = new XMLHttpRequest();
            request.open("GET", "https://authentification.usherbrooke.ca/api/user/" + userNameInput.value.trim() + "/upn", true);

            request.onload = function () {
                if (this.readyState === 4) {
                    if (this.status !== 200) {
                        console.error("No upn found for " + userNameInput.value);
                        resolve(false);
                        return;
                    }

                    var data = JSON.parse(this.responseText);

                    if (data === undefined || data.upn === undefined) {
                        console.error("upn is undefined!");
                        resolve(false);
                        return;
                    }

                    var upn = data.upn.toString();

                    if (upn.indexOf(",") !== -1) {
                        console.error("more than one upn for the username " + userNameInput.value + " specified!");
                        resolve(false);
                        return;
                    }

                    console.log("change username " + userNameInput.value + " for corresponding upn: " + upn);
                    userNameInput.value = upn;

                    resolve(true);
                }
            }

            try {
                request.send();
            } catch (e) {
                console.error("An error occurred while fetching user principal name with error : " + e.toString());

                resolve(false);
            }
        });
    };


    /**
     * Validates login fields executing {@link identity} and
     * {@link appendDomainToUsername} if identity failed.
     *
     * Currently, there is a username validation / transformation that is
     * applied to support multiple username per account.
     *
     * @returns {Promise<boolean>} {@code true} if the validation succeeded,
     * {@code false} otherwise.
     *
     * @see identity
     * @see appendDomainToUsername
     */
    var validateLogin = function () {
        // Find the UPN for current userName value, if not, append domain name
        // to username and try again.
        return identity().then(function (value) {
            return value || (appendDomainToUsername() && identity());
        });
    };

    /**
     * Submits login form depending on current mode.  If the
     * {@link PaginationManager} is present, it triggers the next page.
     * Otherwise it uses the {@code Login} to submit the form.  If neither of
     * them is available, an error is logged.
     *
     * @returns {boolean} {@code true} if the form submit worked, {@code false}
     * if an error occurred.
     */
    var submitLoginForm = function () {
        if (PaginationManager !== undefined) {
            return PaginationManager.validateAndNext();
        }

        if (Login !== undefined) {
            return Login.submitLoginRequest();
        }

        console.error(
            "Could not submit form because the required helper functions " +
            "were not defined");

        return false;
    };

    /**
     * Validates login form and submit.
     *
     * @param {KeyboardEvent} e
     */
    var validateLoginAndSubmit = function (e) {
        if (e.keyCode == 13) {
            validateLogin().then(function (value) {
                return submitLoginForm();
            });
        }
    };

    // Check whether the loginMessage element is present on this page.
    var loginMessage = document.getElementById('loginMessage');
    if (loginMessage) {
        // loginMessage element is present, modify its properties.
        loginMessage.innerHTML = '<p class="title">Connexion</p><p>Identifiant</p>';
    }

    var errorText = document.getElementById('errorText');
    if (errorText) {
        errorText.innerHTML = 'Mauvaise combinaison CIP / mot de passe';
    }

    /**
     * @type {HTMLInputElement}
     */
    var passwordInput = document.getElementById(Login.passwordInput);

    /**
     * @type {HTMLInputElement}
     */
    var userNameInput = document.getElementById(Login.userNameInput);

    var submitButton = document.getElementById('submitButton');

    var kmsiInputLabel = document.querySelector('#kmsiArea > label[for="kmsiInput"]');

    if (submitButton) {
        submitButton.innerHTML = 'Me connecter';
    }

    if (kmsiInputLabel) {
        kmsiInputLabel.innerText = 'Maintenir ma connexion';
    }

    if (userNameInput) {
        userNameInput.placeholder = "Adresse courriel ou CIP";
        userNameInput.addEventListener("keypress", validateLoginAndSubmit, true);
        userNameInput.addEventListener("blur", validateLogin, true);
        userNameInput.addEventListener("submit", validateLogin, true);
    }

    if (passwordInput) {
        passwordInput.placeholder = "Mot de passe";
        passwordInput.addEventListener("keypress", validateLoginAndSubmit, true);
    }
})();
//]]>
</script>


    </body>
</html> 

