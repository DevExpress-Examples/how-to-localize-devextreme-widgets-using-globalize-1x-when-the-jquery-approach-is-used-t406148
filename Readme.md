# How to localize DevExtreme widgets using Globalize 1.X when the jQuery approach is used
<!-- run online -->
**[[Run Online]](https://codecentral.devexpress.com/t406148/)**
<!-- run online end -->


<p>To localize DevExtreme widgets, do the following:</p>
<p><br>- Link required dictionaries as described in the following help topic:<br><a href="http://js.devexpress.com/Documentation/Guide/UI_Widgets/Common/Localization/?search=local&version=16_1&approach=jQuery#Link_Dictionaries">Link Dictionaries</a> in v16.1 <br><a href="https://js.devexpress.com/Documentation/16_2/Guide/Widgets/Common/UI_Widgets/Localization_-_Use_Globalize/#Link_Dictionaries">Link Dictionaries</a> in v16.2+<br><br></p>
<p><strong>Note</strong> that the order of references is important.</p>
<p><br>- Reference the DevExtreme localization script:<br><a href="http://js.devexpress.com/Documentation/Guide/UI_Widgets/Common/Localization/?search=local&version=16_1&approach=jQuery#Use_Predefined_Dictionaries">Use Predefined Dictionaries</a> in v16.1<br><a href="https://js.devexpress.com/Documentation/16_2/Guide/Widgets/Common/UI_Widgets/Localization/#Use_Predefined_Dictionaries">Use Predefined Dictionaries</a> in v16.2+<br><br>- Initialize your application after setting the locale:<br><br></p>


```js
$.when(
        ...
    }).then(
        Globalize.load
    ).then(function () {
        Globalize.locale('de');
        // Initialize your application here
    });
```


<p><br>For a more <strong>detailed description</strong>, refer to the following help topic:</p>
<br><a href="http://js.devexpress.com/Documentation/Guide/UI_Widgets/Common/Localization/?version=16_1#Localization">Localization</a> v16.1<br><a href="https://js.devexpress.com/Documentation/16_2/Guide/Widgets/Common/UI_Widgets/Localization_-_Use_Globalize/">Localization</a> v16.2+<br><br><strong>See also:</strong><br><a href="http://js.devexpress.com/Documentation/Guide/UI_Widgets/Common/Localization/?search=local&version=16_1&approach=jQuery#Use_Predefined_Dictionaries">Extend Predefined Dictionaries</a><br><a href="https://github.com/jquery/globalize/blob/master/doc/api/message/load-messages.md">Globalize.formatMessage</a><br><a href="https://github.com/unicode-cldr">Unicode-CLDR repository</a><br><a href="https://www.devexpress.com/Support/Center/Question/Details/T311368">Localized resources for DevExtreme widgets</a>

<br/>


