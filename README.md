# Microsoft Entra ID Group Management: <br/>Membership, Dynamic Groups, Ownership, and Licensing

Microsoft Entra ID 群組管理：<br/>成員、動態群組、擁有者與授權管理

<br/>

---------

<h2>Outline｜專題簡介</h2>

This project demonstrates fundamental group management operations in Microsoft Entra ID, including Microsoft 365 group creation, security group configuration, membership management, dynamic user membership, group ownership, and group-based license assignment.

本專題展示 Microsoft Entra ID 中的基礎群組管理操作，包括 Microsoft 365 群組建立、安全性群組設定、成員管理、動態使用者成員資格、群組擁有者管理，以及群組式授權指派。

The lab explores different approaches to organizing users through assigned and dynamic membership models. A dynamic security group is configured using the userType attribute to automatically include Guest users within the tenant.

本實驗探索 Assigned 與 Dynamic 兩種群組成員管理方式，並透過 userType 屬性建立動態安全性群組，自動將租戶中的 Guest 使用者納入群組。

The project also demonstrates how existing users can be added to groups through different administrative workflows, and how group ownership and Microsoft service licenses can be managed centrally.

本專題同時展示如何透過不同管理流程將既有使用者加入群組，以及如何集中管理群組擁有者與 Microsoft 服務授權。
<br/>

---------

<h2>Key Learning Outcomes｜主要學習成果</h2>

* Create and configure Microsoft 365 groups in Microsoft Entra ID<br/>
建立與設定 Microsoft Entra ID 中的 Microsoft 365 群組

* Create security groups for identity and access management<br/>
建立用於身分與存取管理的安全性群組

* Understand assigned and dynamic group membership models<br/>
理解 Assigned 與 Dynamic 群組成員管理模式

* Configure dynamic membership rules based on user attributes<br/>
依據使用者屬性設定動態成員資格規則

* Automatically group Guest users using the userType attribute<br/>
使用 userType 屬性自動將 Guest 使用者納入群組

* Add existing users to groups through different administrative workflows<br/>
透過不同管理流程將既有使用者加入群組

* Manage group owners in Microsoft Entra ID<br/>
管理 Microsoft Entra ID 群組擁有者

* Assign Microsoft service licenses to groups<br/>
為群組指派 Microsoft 服務授權

* Understand how group-based administration supports centralized identity management<br/>
理解群組式管理如何支援集中式身分管理
<br/>

---------

<h2>Tools and Concepts Covered｜涵蓋工具與概念</h2>

| Category 分類                                      | Tools / Concepts 工具 / 概念       |
| ------------------------------------------------ | ------------------------------ |
| Cloud Identity Management <br/>雲端身分管理          | Microsoft Entra ID |
| Group Management <br/>群組管理                      | Microsoft Entra Groups |
| Collaboration Groups <br/>協作群組                  | Microsoft 365 Groups |
| Security Groups <br/>安全性群組                      | Microsoft Entra Security Groups |
| Membership Management <br/>成員管理                 | Assigned membership<br/>指派式成員資格 |
| Dynamic Membership <br/>動態成員管理                 | Dynamic User membership<br/>動態使用者成員資格 |
| Dynamic Membership Rules <br/>動態成員規則           | userType Equals Guest |
| External Identity Management <br/>外部身分管理        | Guest user grouping<br/>Guest 使用者群組管理 |
| Group Ownership <br/>群組擁有者管理                  | Group Owners |
| User Membership <br/>使用者群組成員資格              | Add members, Add memberships<br/>新增成員、加入群組 |
| License Management <br/>授權管理                    | Group-based license assignment<br/>群組式授權指派 |
| Microsoft 365 Administration <br/>Microsoft 365 管理 | Microsoft 365 Admin Center |
| Identity Administration <br/>身分管理                | Microsoft Entra Admin Center |


<br/>

---------

<h2>Materials and Methods｜材料與方法</h2>

[Environment]

* Microsoft Azure Portal (Azure 雲端管理平台)</b>
* Microsoft Entra ID tenant (Entra ID 租戶環境)</b>
* Microsoft Entra ID P2 - Trial (Microsoft Entra ID P2 - 試用版)</b>
* Microsoft Entra admin center (Microsoft Entra 管理中心)</b>
* Microsoft 365 admin center (Microsoft 365 管理中心)</b>

[Tasks]

* Create a Microsoft 365 Group (建立 Microsoft 365 群組)
* Create a Dynamic Security Group for Guest Users (建立 Guest 使用者動態安全性群組)
* Add an Existing User to a Group (將既有使用者加入群組)
* Add Owners and Licenses to a Group (在群組中新增所有者和許可證)
<br/>

---------

<h2>Practice｜實踐</h2> <p align="center">

<p align="center">
<b>Task 1: Create a Microsoft 365 Group<br/> (建立 Microsoft 365 群組)</b><br/>
<img src="https://i.imgur.com/dhe9tXZ.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Created a Microsoft 365 group with assigned membership and added an existing user as a group member.<br/>
建立使用 Assigned 成員資格的 Microsoft 365 群組，並將既有使用者加入群組<br/>
<br />
<br />
<b>Task 2-1: Create a Dynamic Security Group<br/> (建立動態安全性群組)</b><br/>
<img src="https://i.imgur.com/UXhnRP8.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Created a security group with Dynamic User membership and configured a rule to <br/>automatically include users whose userType equals Guest.<br/>
建立使用 Dynamic User 成員資格的安全性群組，並設定規則自動納入 userType 屬於 Guest 的使用者<br/>
<br />
<br />
<b>Task 2-2: Validate Dynamic Group Membership<br/> (驗證動態群組成員)</b><br/>
<img src="https://i.imgur.com/T6w1LCV.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Verified that Guest users were automatically populated into the dynamic security group <br/>based on the configured membership rule.<br/>
驗證 Guest 使用者已依據設定的動態成員規則自動加入安全性群組<br/>
<br />
<br />
<b>Task 3: Add an Existing User to a Group<br/> (將既有使用者加入群組)</b><br/>
<img src="https://i.imgur.com/JWzpzk2.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Added an existing external user to the Microsoft 365 group through assigned group membership.<br/>
透過 Assigned 群組成員資格，將既有外部使用者加入 Microsoft 365 群組<br/>
<br />
<br />
<b>Task 4-1: Add an Owner to a Group<br/> (新增群組擁有者)</b><br/>
<img src="https://i.imgur.com/65gtwYN.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Added an existing user as an owner of the Microsoft 365 group to demonstrate delegated group administration.<br/>
將既有使用者新增為 Microsoft 365 群組擁有者，以示範群組管理權限委派<br/>
<br />
<br />
<b>Task 4-2: Assign a License to a Group<br/> (為群組指派授權)</b><br/>
<img src="https://i.imgur.com/wxlnFWW.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Assigned Microsoft Entra ID P2 to the Project23 Microsoft 365 group through Microsoft Graph and <br/>verified the group-based license assignment in the Microsoft 365 Admin Center.<br/>
透過 Microsoft Graph 將 Microsoft Entra ID P2 指派給 Project23 Microsoft 365 群組，<br/>並於 Microsoft 365 Admin Center 驗證群組式授權結果<br/>
<br />
<br />


---------

<h2>Results｜專題結論</h2>

This project demonstrated the administration of users, Microsoft 365 groups, group membership, and license provisioning within a Microsoft Entra environment. By using the Project23 group as a centralized management object, administrative tasks could be applied consistently at the group level rather than managed separately for individual users.

本專題實作 Microsoft Entra 環境中的使用者、Microsoft 365 群組、群組成員及授權配置管理。透過 Project23 群組作為集中式管理物件，可將管理作業一致地套用至群組，而非逐一管理個別使用者。

We also involved troubleshooting differences between Microsoft Entra tenants and limitations in the current Microsoft 365 Admin Center interface. Microsoft Graph was used to verify group properties and complete the Microsoft Entra ID P2 group-based license assignment, with the result subsequently validated through the Microsoft 365 Admin Center.

我們也檢視了 Microsoft Entra 租用戶之間的差異以及目前 Microsoft 365 管理中心介面存在的限制。透過 Microsoft Graph 驗證群組屬性並完成 Microsoft Entra ID P2 群組式授權指派，最後再回到 Microsoft 365 Admin Center 驗證實際結果。

<br />
<br />



---------

<h2>Security Insight｜安全洞察</h2>


Group-based identity and license management improves consistency, scalability, and auditability by associating access and service entitlements with managed groups instead of relying on repeated manual changes to individual accounts. This approach can reduce configuration errors and support more structured user lifecycle and access governance processes.

基於群組的身份和許可證管理透過將存取權限和服務授權與受管群組關聯，而非依賴對單一帳戶的重複手動更改，從而提高了一致性、可擴展性和可稽核能力。這種方法可以減少配置錯誤，並支援更結構化的使用者生命週期和存取治理流程。

The troubleshooting process also demonstrated that administrative roles, tenant boundaries, object properties, and application permissions are separate security controls. Holding the Global Administrator role does not automatically grant an application such as Microsoft Graph Explorer every API permission, while users, groups, licenses, and roles remain isolated between different Microsoft Entra tenants. Understanding these boundaries is important when diagnosing IAM issues and applying least-privilege administration.

本次故障排除亦呈現出管理角色、Tenant 邊界、物件屬性與應用程式權限屬於不同的安全控制層級。即使帳號具備 Global Administrator 角色，也不代表 Microsoft Graph Explorer 自動擁有所有 API 權限；不同 Microsoft Entra Tenant 之間的使用者、群組、授權與角色亦彼此隔離。理解這些安全邊界，是進行 IAM 問題診斷及落實最小權限管理的重要基礎。


<br />
<br />

---------

<h2>Reference｜參考</h2>

* [Microsoft] [Microsoft Certified: Identity and Access Administrator Associate (SC-300)](https://learn.microsoft.com/en-us/credentials/certifications/identity-and-access-administrator/?practice-assessment-type=certification)<br/>
* [Microsoft] [Get started with identity and access labs](https://learn.microsoft.com/en-au/training/modules/get-started-identity-access-labs/)<br/>
<br/>
