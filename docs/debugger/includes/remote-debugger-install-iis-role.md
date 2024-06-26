---
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
These steps show only a basic configuration of IIS. For more in-depth information or to install to a Windows Desktop machine, see [Publishing to IIS](/aspnet/core/publishing/iis?tabs=aspnetcore2x#iis-configuration) or [IIS 8.0 Using ASP.NET 3.5 and ASP.NET 4.5](/iis/get-started/whats-new-in-iis-8/iis-80-using-aspnet-35-and-aspnet-45).

For Windows Server operating systems, use the **Add Roles and Features** wizard via the **Manage** link or the **Dashboard** link in **Server Manager**. On the **Server Roles** step, check the box for **Web Server (IIS)**.

![Screenshot showing the Web Server IIS role selected in the Select server roles step.](../media/remote-debug-server-roles-ws2022.png)

(Windows Server 2022) In the dialog box that appears, choose **Add Features** to add the IIS Management Console.

On the **Role services** step, select the IIS role services you desire or accept the default role services provided. If you want to enable deployment using publish settings and Web Deploy, make sure that the following features are selected:

- **IIS Management Scripts and Tools**
- **Management Service**
- **IIS Management Console**

![Screenshot showing IIS Management scripts and tools selected.](../media/remote-debug-server-config-add-scripts-and-tools.png)

Proceed through the confirmation steps to install the web server role and services. A server/IIS restart is not required after installing the Web Server (IIS) role.