<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <title>Extended EMail Action Plugin</title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
    <meta http-equiv="X-UA-Compatible" content="IE=EmulateIE8" />
    <meta content="Scroll Wiki Publisher" name="generator"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/liquid.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/print.css" media="print"/>
    <link type="text/css" rel="stylesheet" href="css/content-style.css" media="screen, projection, print"/>
    <link type="text/css" rel="stylesheet" href="css/screen.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/print.css" media="print"/>
</head>
<body>
                <h1>Extended EMail Action Plugin</h1>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-Overview"  >
        <h2>Overview</h2>
    <p>
    </p>
            <img src="images_community/download/attachments/120128619/icon.png" alt="images_community/download/attachments/120128619/icon.png" class="confluence-embedded-image" />
            <p>
This plugin provides more flexibility when it comes to sending email action alerts. You have full control over the email message that gets send and can also specify additional filtering options e.g: just send the email when the Incident comes from a specific agent or server    </p>
    <p>
    </p>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-PluginDetails"  >
        <h2>Plugin Details</h2>
    <div class="tablewrap">
        <table>
<thead class=" "></thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Author    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Eugene Turetsky (Eugene.Turetsky@compuware.com)    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
dynaTrace Versions    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
dynaTrace 4.2, 5.0+    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
License    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_5275722_2_dynaTraceBSD.txt">dynaTrace BSD</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Support    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="https://community/display/DL/Support+Levels">Not Supported</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Known Problems    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Release History    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
2013-07-05 Initial Release 0.9.5,    </p>
    <p>
2013-08-07 Release 0.9.6    </p>
    <p>
2013-10-10 Release 0.9.7    </p>
    <p>
2013-12-27 Release 0.9.8    </p>
    <p>
2014-02-26 Release 0.9.9.5    </p>
    <p>
2014-07-01 Release 0.9.9.6    </p>
    <p>
2014-07-22 Release 0.9.9.7    </p>
    <p>
2014-09-16 Release 0.9.9.8 - 0.9.9.9 (beta)    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Download    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_178487990_1_com.dynatrace.diagnostics.plugins.extendedmailreport_0.9.9.10.jar">com.dynatrace.diagnostics.plugins.extendedmailreport_0.9.9.10.jar</a>    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-NewintheRelease0.9.9.8-0.9.9.10"  >
        <h2>New in the Release 0.9.9.8 - 0.9.9.10</h2>
    <p>
New features include:    </p>
<ul class=" "><li class=" ">    <p>
Ability to send notification e-mails to different addresses depending on filters criteria. The list of filters and correspondent e-mails will be provided in the XML file. Please see example of the XML file <a href="attachments_178487574_1_filters.xml">here</a>. The matching XSD schema file is located <a href="attachments_178487575_1_filters.xsd">here</a>. Plugin internally validates XML file using this schema. Please use the following link to validate correctness of the XML file outside of the plugin: <a href="http://www.utilities-online.info/xsdvalidation/#.VBiU600tCUl">XML-validation-link</a>.<br/>There are two new parameters which define if filters/e-mails pairs are used by the plugin They are (see the following <a href="attachments_174754304_1_New-plugins-parameters.png">screenshot</a>):    </p>
<ul class=" "><li class=" ">    <p>
Are Emails and Filters Coupled;    </p>
</li><li class=" ">    <p>
Emails-Filters Dependency File.    </p>
</li></ul></li><li class=" ">    <p>
Ability to filter by agent names and by server names for the following sources (see the following <a href="attachments_178487577_1_Filters_by_servers.png">screenshot</a> for new parameters):    </p>
<ul class=" "><li class=" ">    <p>
Agents;    </p>
</li><li class=" ">    <p>
Monitors;    </p>
</li><li class=" ">    <p>
Collectors.    </p>
</li></ul></li><li class=" ">    <p>
Mitigated issue with excessive invocations of the Action plugin setup/teardown methods by the dynaTrace engine. Two new properties are added to the extendedmailactionplugin.properties file. They are:    </p>
<ul class=" "><li class=" ">    <p>
expireCacheInterval;    </p>
</li><li class=" ">    <p>
cleanupInterval.    </p>
</li></ul></li></ul>    <p>
These parameters are taken in minutes. The <i class=" ">extendedmailactionplugin.properties</i> file is located in the 'res' subdirectory of the plugin's jar file. Example of the extendedmailactionplugin.properties file is located <a href="attachments_178487578_1_extendedmailactionplugin.properties">here</a>.    </p>
    <p>
There are two new parameters which are added to the plugin to uniquely identify instance of the action plugin. They are:    </p>
<ul class=" "><li class=" "><ul class=" "><li class=" ">    <p>
Incident Rule Name;    </p>
</li><li class=" ">    <p>
Identity String.    </p>
</li></ul></li></ul>    <p>
Please see example of using these parameters <a href="attachments_178487580_1_New_parameters.png">here</a>. While the first parameter is required to identify instance of the plugin which is associated with the specific incident rule, the second parameter is optional and only necessary when there are two or more instances of this plugin setup for a given incident rule. The last scenario of having two or more instances of the Extended Mail Action Plugin (as well as any action plugin) for given incident rule is <i class=" ">highly</i> <i class=" ">discouraged</i> if incidents are thrown frequently. If you have need in having multiple instances of the Extended Mail Action Plugin for a given incident rule, and given version of the plugin does not allow you to cover your needs with a single plugin instance, please contact us to provide your use cases. We will make this plugin (or other action plugins) to accommodate your use cases that you will have to configure just one instance of the plugin per incident rule.    </p>
<ul class=" "><li class=" ">    <p>
Added new configuration parameter ALL_SERVER_NAMES_CAPS: when it is &quot;true&quot;, content of the ${ALL_SERVER_NAMES} environmental variable is in upper case letters, otherwise it is unchanged.    </p>
</li></ul>    <p>
<strong class=" ">Note</strong>    </p>
    <p>
This version of the plugin is a beta version now. It will become a GA release after successful beta testing.    </p>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-NewintheRelease0.9.9.7"  >
        <h2>New in the Release 0.9.9.7</h2>
    <p>
Additional filtering of notification e-mails:    </p>
<ul class=" "><li class=" ">    <p>
Added new configuration parameter sendOnlyPatterns: it is a semicolon separated list of Java regular <a href="http://docs.oracle.com/javase/7/docs/api/java/util/regex/Pattern.html">expressions</a>. Each regular expression from the sendOnlyPatterns list will be evaluated against the following incident variables:    </p>
</li></ul>    <p>
- MESSAGE;<br/>- RULE_DESCRIPTION;<br/>- VIOLATION_HEADER_1;<br/>- VIOLATION_MESSAGE_1;<br/>- VIOLATION_HEADER_2;<br/>- VIOLATION_MESSAGE_2;<br/>- VIOLATION_HEADER_3;<br/>- VIOLATION_MESSAGE_3;<br/>- VIOLATION_HEADER_4;<br/>- VIOLATION_MESSAGE_4;<br/>- VIOLATION_HEADER_5;<br/>- VIOLATION_MESSAGE_5.    </p>
    <p>
Notification e-mail will be sent only if match is found in any of the above variables, otherwise notification e-mail will not be sent.    </p>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-NewintheRelease0.9.9.6"  >
        <h2>New in the Release 0.9.9.6</h2>
    <p>
Added support for e-mail notifications from the Cloud:    </p>
<ul class=" "><li class=" ">    <p>
Added new configuration parameter SmtpUserPassword: when it is on, user name and password must be provided for SMTP mail server.    </p>
</li></ul>    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-NewintheRelease0.9.9.5"  >
        <h2>New in the Release 0.9.9.5</h2>
    <p>
Changes include:    </p>
<ul class=" "><li class=" ">    <p>
Removed port from the Agent_Host/Monitor_Host/Collector_Nost/Server_Host for OOTB incidents;    </p>
</li><li class=" ">    <p>
Improved content of the e-mail body for e-mails in the plain text format;    </p>
</li><li class=" ">    <p>
Added application name in the Details section of the e-mail body where it is available;    </p>
</li><li class=" ">    <p>
Use of incident's message in cases where violations have no meaningful content for OOTB incidents.    </p>
</li></ul>    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-NewintheRelease0.9.9.4"  >
        <h2>New in the Release 0.9.9.4</h2>
    <p>
Added hosts' DNS name to IP address translation for the agents, monitors, collectors, and servers. New predefined variables are added to the list of maintained by the plugin variables:    </p>
<ol class=" "></ol><ul class=" "><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_AGENT_HOSTS_IP_ADDRESSES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_MONITOR_HOSTS_IP_ADDRESSES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_COLLECTOR_HOSTS_IP_ADDRESSES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_SERVER_HOSTS_IP_ADDRESSE</i>S    </p>
</li></ul>    <p>
Provided write-up of the <a href="attachments_154697856_5_Workaround-incident-sensitivity-issue.docx">Workaround of incorrect sensitivity issue for built-in OOTB incidents for dynaTrace action plugins</a>.    </p>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-NewintheRelease0.9.8"  >
        <h2>New in the Release 0.9.8</h2>
    <p>
Added ability to embed into dashboard names predefined variables which will be substituted with their runtime values.    </p>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-NewintheRelease0.9.7"  >
        <h2>New in the Release 0.9.7</h2>
    <p>
Here is list of new features:    </p>
<ul class=" "><li class=" ">    <p>
Added support for plain text e-mail format:    </p>
</li></ul><ul class=" "><li class=" ">    <p>
new parameter &quot;HTML Mail Format&quot; is set to &quot;true&quot; for HTML notifications and &quot;false&quot; for ASCII/Text notifications. Default value is &quot;true&quot;.    </p>
</li></ul><ul class=" "><li class=" ">    <p>
Plugin supports now reports in HTML, PDF, XLS, XML, CSV, and XSD formats:    </p>
<ul class=" "><li class=" ">    <p>
new parameter &quot;Dashboards Type&quot; is set to one of the above report formats.    </p>
</li></ul></li><li class=" ">    <p>
Added new external variables supported by the plugin:    </p>
<ul class=" "><li class=" ">    <p>
DYNATRACE_SERVER_REST_PORT    </p>
</li><li class=" ">    <p>
DASHBOARD_URL_1, DASHBOARD_URL_2,... DASHBOARD_URL_5 provide up to 5 links for dashboards' reports.    </p>
</li></ul></li><li class=" ">    <p>
Added support for &quot;quiet time&quot; when notification e-mails will not be sent. During quiet time incidents will be triggered as they would be during usual activities but notification e-mails will not be sent.    </p>
</li></ul><ul class=" "><li class=" ">    <p>
two new parameters &quot;Quiet Time From&quot; and Quiet Time To&quot; are setting up a quiet time interval.    </p>
</li></ul>    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-NewintheRelease0.9.6"  >
        <h2>New in the Release 0.9.6</h2>
    <p>
Here is list of new features:    </p>
<ul class=" "><li class=" ">    <p>
Significantly improved integration with the OOTB incidents;    </p>
</li><li class=" ">    <p>
Added support for <a href="http://docs.oracle.com/javase/7/docs/api/java/util/regex/Pattern.html">Java regular expressions</a> for filtering incidents by Agents, Agent Groups, Monitors, Collectors, and Servers    </p>
</li><li class=" ">    <p>
Plugin maintains new variables which capture sources of the incidents (AGENT_NAME_1, AGENT_NAME_2, etc.);    </p>
</li><li class=" ">    <p>
Plugin maintains new variables which capture list of incidents&rsquo; sources (ALL_AGENTS, ALL_AGENT_NAMES, ALL_AGENT_HOSTS etc.);    </p>
</li><li class=" ">    <p>
Plugin provides REST filtering of the PDF reports by agent names/hosts, group names, and/or custom timeframe;    </p>
</li><li class=" ">    <p>
START_TIME and END_TIME variables are set to &ldquo;-&ldquo; if they are not defined;    </p>
</li><li class=" ">    <p>
Separator for multiple incident&rsquo;s sources for filtering set to semicolon (&ldquo;;&rdquo;).    </p>
</li></ul>    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-Installation"  >
        <h2>Installation</h2>
    <p>
Import the Plugin into the dynaTrace Server. For details how to do this please refer to the <a href="https://community/display/DOCDT42/Plugin+Management">Online Documentation on Plugin Management</a>.    </p>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-Usage"  >
        <h2>Usage</h2>
    <p>
The plugin was originally shared through the following discussion forum entry: <a href="https://community/display/DTFORUM/Automatic+Dash+Report+via+e-mail">Automatic Dash Report via e-mail</a>.<br/>The following link contains documentation for the plugin: <strong class=" "><a href="attachments_156632431_1_Extended_Mail_Action_Plugin_Release_0.9.9.2.docx">Extended Mail Action Plugin</a>.</strong>    </p>
    <p>
The Extended Email Report Action Plugin has the following features:    </p>
<ol class=" "><li class=" ">    <p>
Filtering of incidents based on    </p>
<ol class=" "><li class=" ">    <p>
agents    </p>
</li><li class=" ">    <p>
agent groups    </p>
</li><li class=" ">    <p>
monitors    </p>
</li><li class=" ">    <p>
collectors    </p>
</li><li class=" ">    <p>
servers    </p>
</li></ol></li><li class=" ">    <p>
Customize Subject and Body of the e-mail    </p>
<ol class=" "><li class=" ">    <p>
Add/replace Subject and/or Body of the OOTB e-mail which is generated by the Email Alert Action plugin    </p>
</li></ol></li><li class=" ">    <p>
Embed predefined variables into the customized text in order to provide incident's details at runtime in the Subject and/or Body of the e-mail. This list consist of the following variables:    </p>
</li></ol><ul class=" "><li class=" ">    <p>
<i class=" ">AGENT_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_NAME_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_NAME_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_NAME_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_NAME_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_NAME_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_HOST_IP_ADDRESS_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_AGENT_NAMES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_AGENT_HOSTS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_AGENT_HOSTS_IP_ADDRESSES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_AGENTS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_GROUP_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_GROUP_NAME_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_GROUP_NAME_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_GROUP_NAME_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_GROUP_NAME_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">AGENT_GROUP_NAME_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_AGENT_GROUP_NAMES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_NAME_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_NAME_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_NAME_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_NAME_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_NAME_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">MONITOR_HOST_IP_ADDRESS_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_MONITOR_NAMES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_MONITOR_HOSTS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_MONITOR_HOSTS_IP_ADDRESSES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_MONITORS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_NAME_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_NAME_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_NAME_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_NAME_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_NAME_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">COLLECTOR_HOST_IP_ADDRESS_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_COLLECTOR_NAMES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_COLLECTOR_HOSTS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_COLLECTOR_HOSTS_IP_ADDRESSES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_COLLECTORS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_NAME_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_NAME_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_NAME_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_NAME_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_NAME_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SERVER_HOST_IP_ADDRESS_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_SERVER_HOSTS_IP_ADDRESSE</i>S    </p>
</li><li class=" ">    <p>
<i class=" ">ALL_SERVER_NAMES</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">DYNATRACE_SERVER_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">DYNATRACE_SERVER_REST_PORT,</i>    </p>
</li><li class=" ">    <p>
<i class=" ">MESSAGE</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">RULE_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">RULE_DESCRIPTION</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SENSITIVITY</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SESSION_ID</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SESSION_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">START_TIME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">END_TIME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">DURATION</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">IS_OPEN</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">IS_CLOSED</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SEVERITY</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">KEY</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">STATE</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">SYSTEM_PROFILE</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">APPLICATION</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_DESCRIPTION</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_VALUE</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_UNIT</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_SPLITTINGS</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_TRESHOLD_UPPER_SEVERE</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_TRESHOLD_LOWER_SEVERE</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_TRESHOLD_UPPER_WARNING</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_TRESHOLD_LOWER_WARNING</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_METRIC_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_METRIC_DESCRIPTION</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_METRIC_GROUP</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_MEASURE_METRIC_UNIT</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_TRIGGER_VALUE_SOURCE_TYPE</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_TRIGGER_VALUE_SOURCE_NAME</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_TRIGGER_VALUE_SOURCE_HOST</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATED_TRIGGER_VALUE</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATION_HEADER_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATION_MESSAGE_1</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATION_HEADER_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATION_MESSAGE_2</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATION_HEADER_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATION_MESSAGE_3</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATION_HEADER_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATION_MESSAGE_4</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATION_HEADER_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">VIOLATION_MESSAGE_5</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">INCIDENT_STARTED_ENDED</i>,    </p>
</li><li class=" ">    <p>
<i class=" ">IMAGE_WARNING_OK,</i>    </p>
</li><li class=" ">    <p>
<i class=" ">DASHBOARD_URL_1,</i>    </p>
</li><li class=" ">    <p>
<i class=" ">DASHBOARD_URL_2,</i>    </p>
</li><li class=" ">    <p>
<i class=" ">DASHBOARD_URL_3,</i>    </p>
</li><li class=" ">    <p>
<i class=" ">DASHBOARD_URL_4,</i>    </p>
</li><li class=" ">    <p>
<i class=" ">DASHBOARD_URL_5.</i><i class=" "> </i><br/>    <span style="color: #000000;">
     </span>
    </p>
</li></ul><ul class=" "><li class=" ">    <p>
Attach multiple custom and/or OOTB dashboards in PDF format    </p>
<ol class=" "><li class=" ">    <p>
Filter reports using agent-names/agent-hosts, agent-groups, and/or custom timeframe    </p>
</li></ol></li><li class=" ">    <p>
Customize To, CC, and BCC fields of the e-mail by providing lists of e-mail addresses    </p>
</li><li class=" ">    <p>
Set From e-mail address    </p>
</li><li class=" ">    <p>
Set specific SMTP mail server    </p>
</li></ul>    <p>
The plugin provides a great extension to the default Email Alert Action plugin.    </p>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-Configuration"  >
        <h2>Configuration</h2>
    <p>
The following screenshot shows an example configuration for non-SSL SMTP server.             <img src="images_community/download/attachments/120128619/configuration_example_1.png" alt="images_community/download/attachments/120128619/configuration_example_1.png" class="confluence-embedded-image confluence-content-image-border" />
    <br/><br/>Next screenshot shows an example configuration for SSL SMTP server:             <img src="images_community/download/attachments/120128619/configuration_example_2.png" alt="images_community/download/attachments/120128619/configuration_example_2.png" class="confluence-embedded-image confluence-content-image-border" />
            </p>
    <p>
Next screenshot shows Report Filtering by Agent Name/Agent Host, Agent Group, and Custom Timeframe:            <img src="images_community/download/attachments/120128619/rest-filters.png" alt="images_community/download/attachments/120128619/rest-filters.png" class="confluence-embedded-image" />
        </p>
    <p>
    </p>
    <p>
Next screenshot shows an example configuration of the Body parameter:             <img src="images_community/download/attachments/120128619/Body_Example_1.png" alt="images_community/download/attachments/120128619/Body_Example_1.png" class="confluence-embedded-image confluence-content-image-border" />
        </p>
    <p>
Next screenshot contains more complex example of the Body parameter (full content of the Body parameter is <a href="attachments_154697847_1_BodyExample.html">here</a>):            <img src="images_community/download/attachments/120128619/BodyExample_02-01-2014.png" alt="images_community/download/attachments/120128619/BodyExample_02-01-2014.png" class="confluence-embedded-image" />
        <br/>Next screenshot shows e-mail which was created by the Body depicted in the previous screenshot:            <img src="images_community/download/attachments/120128619/Body_Example1_view_updated.png" alt="images_community/download/attachments/120128619/Body_Example1_view_updated.png" class="confluence-embedded-image" />
        <br/>For more examples of Body, Body Header, and Body Footer parameters please see pages 11 - 13 of the <a href="attachments_121569655_15_Extended_Mail_Action_Plugin.docx"><strong class=" ">Extended Mail Action Plugin</strong></a> document.    </p>
    <p>
Next screenshot shows an example configuration of filtering by agents:             <img src="images_community/download/attachments/120128619/configuration_example_3.png" alt="images_community/download/attachments/120128619/configuration_example_3.png" class="confluence-embedded-image confluence-content-image-border" />
    <br/>For more details about filtering see section 2 on page 7 of the <strong class=" "><a href="attachments_132120588_7_Extended_Mail_Action_Plugin_Release_0.9.6.docx">Extended Mail Action Plugin</a></strong> document.    </p>
    <p>
Next screenshot shows an example configuration for generating and attaching PDF files to the e-mail:             <img src="images_community/download/attachments/120128619/configuration_example_4.png" alt="images_community/download/attachments/120128619/configuration_example_4.png" class="confluence-embedded-image confluence-content-image-border" />
        </p>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-CustomText"  >
        <h2>Custom Text</h2>
    <p>
The following notation is used to embed predefined variables in the text:    </p>
<ul class=" "><li class=" ">    <p>
${variable-name}, where variable-name is one of the names from the list of predefined variables.    </p>
</li></ul>    <p>
Next is an example of custom text:    </p>
    <p>
&quot;I do not like incidents, especially when they are coming from the agent ${AGENT_NAME} which is running on the host ${AGENT_HOST}&quot;    </p>
    <p>
For more examples see section 4 on page 9 of the <strong class=" "><a href="attachments_132120588_7_Extended_Mail_Action_Plugin_Release_0.9.6.docx">Extended Mail Action Plugin</a></strong> document.    </p>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-"  >
        <h2></h2>
    </div>
    <div class="section-2"  id="120128619_ExtendedEMailActionPlugin-Feedback"  >
        <h2>Feedback</h2>
    <p>
Please provide feedback on this plugin either by commenting on this page or by comments on the <a href="https://community/display/DTFORUM/Community+Plugins+and+Extensions">Community Plugins and Extensions</a>    </p>
    <p>
    </p>
    <p>
    </p>
    </div>
            </div>
        </div>
        <div class="footer">
        </div>
    </div>
</body>
</html>