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

---------

<h2>Results｜專題結論</h2>

This project provided practical experience with fundamental identity and user administration tasks in Microsoft Entra ID. The workflow covered user provisioning, sign-in validation, service license assignment, external guest onboarding, directory role assignment, and bulk user creation.

本專題提供 Microsoft Entra ID 基礎身分與使用者管理的實務操作經驗，流程涵蓋使用者帳號建立、登入驗證、服務授權指派、外部 Guest 使用者建立、目錄角色指派，以及批次使用者建立。

The project demonstrated that identity administration involves more than simply creating user accounts. User properties such as usage location, user type, licensing status, and assigned directory roles can directly affect the services and administrative capabilities available to each identity. External user invitation demonstrated how Microsoft Entra ID supports collaboration with identities outside the organization while maintaining a separate Guest user classification within the tenant. The directory role exercises also demonstrated multiple administrative workflows for assigning built-in Microsoft Entra roles, while bulk user provisioning introduced a more scalable approach to creating multiple identities through CSV-based operations.

本專題展示身分管理不僅是建立使用者帳號，Usage Location、User Type、License 狀態以及目錄角色等使用者屬性，都可能直接影響身分可使用的服務與管理權限。外部使用者邀請流程則展示 Microsoft Entra ID 如何支援組織外部身分進行協作，同時透過 Guest 使用者類型在租戶中維持不同的身分分類。目錄角色實作展示了使用不同管理介面指派 Microsoft Entra 內建角色的方式；批次使用者建立則進一步導入以 CSV 為基礎的大量帳號建立流程，提升使用者管理的可擴展性。

Overall, the project demonstrated a basic identity lifecycle workflow in Microsoft Entra ID, from initial account provisioning and service enablement to external collaboration, administrative delegation, and scalable user management.

整體而言，本專題展示了 Microsoft Entra ID 中基礎的身分生命週期管理流程，從帳號建立與服務啟用，到外部協作、管理權限委派，以及可擴展的使用者管理方式。

<br />
<br />

<br />
<br />


---------

<h2>Security Insight｜安全洞察</h2>


Identity Lifecycle Management (身分生命週期管理)

User provisioning should be treated as part of an identity lifecycle rather than as an isolated account creation task. Creating an identity, validating access, assigning required services, reviewing privileges, and managing the account at scale are interconnected administrative activities.

使用者建立應視為身分生命週期的一部分，而非單純的帳號建立操作。建立身分、驗證存取、指派所需服務、檢視權限，以及大量管理帳號，皆屬於彼此關聯的身分管理流程。


User Attributes and Service Access (使用者屬性與服務存取)

Identity attributes can directly affect access to cloud services. During the lab, license assignment depended on the user having a valid Usage Location, demonstrating that incomplete or incorrect identity properties can cause downstream access and provisioning failures.

身分屬性會直接影響雲端服務的存取與配置。本實驗中，License 指派需要使用者具備有效的 Usage Location，說明不完整或錯誤的身分屬性可能導致後續的存取與服務配置失敗。


External Identity Management (外部身分管理)

Microsoft Entra ID allows external collaborators to be represented as Guest users within the tenant. Separating external identities from internal Members helps administrators apply different access policies and maintain clearer visibility over users who originate outside the organization.

Microsoft Entra ID 可將外部協作者以 Guest 使用者形式建立於租戶中。將外部身分與內部 Member 分類管理，有助於套用不同的存取政策，並提升對組織外部使用者的可視性。


Role-Based Administrative Delegation (角色式管理權限委派)

Directory roles allow administrative permissions to be delegated according to operational responsibilities rather than granting unrestricted administrative access. Built-in roles provide a structured way to separate responsibilities and support the principle of least privilege.

目錄角色可依據實際管理職責委派行政權限，而非直接授予不受限制的管理權限。Microsoft Entra 內建角色提供結構化的權限分工方式，有助於實踐最小權限原則。


Bulk Provisioning and Validation (批次建立與驗證)

Bulk user creation improves scalability but also increases the impact of configuration errors. CSV-based provisioning should therefore be followed by validation of bulk operation results and the resulting user objects instead of assuming that a successful submission means every account was created successfully.

批次建立使用者能提升管理效率，但設定錯誤的影響範圍也會同步擴大。因此使用 CSV 進行大量帳號建立後，應進一步驗證 Bulk Operation 結果與實際產生的使用者物件，而不能僅依據提交成功訊息判斷所有帳號皆已建立完成。


Administrative Verification (管理操作驗證)

Identity administration should include verification after each significant change. Sign-in testing, reviewing assigned licenses, confirming Guest user type, checking directory role assignments, and validating bulk-created accounts help ensure that configuration changes produce the intended result.

身分管理中的重要變更完成後應進行驗證。透過登入測試、確認 License 狀態、驗證 Guest 使用者類型、檢查目錄角色，以及確認批次建立帳號結果，可確保實際設定符合原先預期。


<br />
<br />

---------

<h2>Reference｜參考</h2>

* [Microsoft] [Microsoft Certified: Identity and Access Administrator Associate (SC-300)](https://learn.microsoft.com/en-us/credentials/certifications/identity-and-access-administrator/?practice-assessment-type=certification)<br/>
* [Microsoft] [Get started with identity and access labs](https://learn.microsoft.com/en-au/training/modules/get-started-identity-access-labs/)<br/>
<br/>
