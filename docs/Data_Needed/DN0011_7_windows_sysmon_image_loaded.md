| Title              | DN0011_7_windows_sysmon_image_loaded       |
|:-------------------|:------------------|
| **Author**         | @atc_project        |
| **Description**    | The image loaded event logs when a module is loaded in a specific process |
| **Logging Policy** | <ul><li>[LP0006_windows_sysmon_image_loaded](../Logging_Policies/LP0006_windows_sysmon_image_loaded.md)</li></ul> |
| **References**     | <ul><li>[https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/event.aspx?eventid=90007](https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/event.aspx?eventid=90007)</li><li>[https://github.com/Cyb3rWard0g/OSSEM/blob/master/data_dictionaries/windows/sysmon/event-7.md](https://github.com/Cyb3rWard0g/OSSEM/blob/master/data_dictionaries/windows/sysmon/event-7.md)</li></ul> |
| **Platform**       | Windows    |
| **Type**           | Applications and Services Logs        |
| **Channel**        | Microsoft-Windows-Sysmon/Operational     |
| **Provider**       | Microsoft-Windows-Sysmon    |
| **Fields**         | <ul><li>EventID</li><li>Computer</li><li>Hostname</li><li>UtcTime</li><li>ProcessGuid</li><li>ProcessId</li><li>Image</li><li>ImageLoaded</li><li>FileVersion</li><li>Description</li><li>Product</li><li>Company</li><li>OriginalFileName</li><li>Hashes</li><li>Signed</li><li>Signature</li><li>SignatureStatus</li></ul> |


## Log Samples

### Raw Log

```
- <Event xmlns="http://schemas.microsoft.com/win/2004/08/events/event">
  - <System>
    <Provider Name="Microsoft-Windows-Sysmon" Guid="{5770385F-C22A-43E0-BF4C-06F5698FFBD9}" /> 
    <EventID>7</EventID> 
    <Version>3</Version> 
    <Level>4</Level> 
    <Task>7</Task> 
    <Opcode>0</Opcode> 
    <Keywords>0x8000000000000000</Keywords> 
    <TimeCreated SystemTime="2019-07-09T04:15:07.860831900Z" /> 
    <EventRecordID>9146</EventRecordID> 
    <Correlation /> 
    <Execution ProcessID="1540" ThreadID="3456" /> 
    <Channel>Microsoft-Windows-Sysmon/Operational</Channel> 
    <Computer>atc-win-10</Computer> 
    <Security UserID="S-1-5-18" /> 
  </System>
  - <EventData>
    <Data Name="RuleName" /> 
    <Data Name="UtcTime">2019-07-09 04:13:59.602</Data> 
    <Data Name="ProcessGuid">{717CFEC0-1487-5D24-0000-00103F202900}</Data> 
    <Data Name="ProcessId">2352</Data> 
    <Data Name="Image">C:\Windows\System32\sihost.exe</Data> 
    <Data Name="ImageLoaded">C:\Windows\System32\msvcrt.dll</Data> 
    <Data Name="FileVersion">7.0.14393.0 (rs1_release.160715-1616)</Data> 
    <Data Name="Description">Windows NT CRT DLL</Data> 
    <Data Name="Product">Microsoft® Windows® Operating System</Data> 
    <Data Name="Company">Microsoft Corporation</Data> 
    <Data Name="OriginalFileName">msvcrt.dll</Data> 
    <Data Name="Hashes">MD5=94EF9321C287FC1B179419E662996A41,SHA256=555B434EC9E8628820905A8F1D7BC7F8EE99C6D44A01892ADD16E39E6B675A0D</Data> 
    <Data Name="Signed">true</Data> 
    <Data Name="Signature">Microsoft Windows</Data> 
    <Data Name="SignatureStatus">Valid</Data> 
  </EventData>
</Event>

```




