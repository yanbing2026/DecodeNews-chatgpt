<<<CDB_ZH>>>
# Microsoft Entra ID的MemberOf规则运算符于11月3日退役，企业需检查动态组配置

Microsoft 提醒 Microsoft Entra ID 管理员，MemberOf 规则运算符的公开预览功能将于2026年11月3日退役。使用该运算符的动态成员组、动态管理单元和权限管理自动分配策略将停止处理成员变更。若企业未提前替换规则，用户可能无法获得应有的访问权限或许可证，离职人员也可能继续保留本应撤销的权限。

## 退役日期为11月3日

Microsoft 365 Message Center 的最终提醒指出，MemberOf 运算符将于11月3日停止工作。该功能此前处于公开预览阶段，Microsoft 表示，测试发现它可能影响同一租户内动态成员处理的规模和可靠性，即使只存在一条 MemberOf 规则，也可能对处理过程造成影响。因此公司决定结束预览，而不是将其作为正式生产功能继续支持。

## 动态组成员更新将停止

Microsoft 的通知称，退役后，包含 MemberOf 的动态组将不再处理成员变更；动态管理单元也不会继续更新成员和管理范围。使用该运算符的 Entitlement Management 自动分配策略同样会停止处理分配更新。已有成员关系和分配数据会保留在最后一次已知状态，而不是自动清空。

## 过期权限可能形成安全风险

如果动态组不再更新，新加入组织的员工可能无法获得所需应用访问或许可证；离职员工则可能继续保留本应撤销的访问权限。依赖动态组成员关系的 Conditional Access 策略、Teams、SharePoint 和基于组的许可证分配，也可能使用过期信息。Microsoft 因此建议管理员在退役前检查所有相关配置。

## 管理员需要替换规则或改为指定成员

Microsoft 建议企业导出动态成员组清单，识别包含 MemberOf 的规则，并在可行时替换为受支持的规则运算符。如果没有可用替代规则，管理员应考虑将组转换为 assigned membership。动态管理单元和 Entitlement Management 自动分配策略也需要逐项检查，并在修改后验证成员、权限范围和访问包分配结果。

## 影响范围不仅是单一组功能

MemberOf 规则可能被用于访问控制、许可证分配和管理范围判断，因此停用会影响依赖动态成员变化的多个系统。企业应检查 Conditional Access 是否依赖相关动态组，并确认新员工和离职员工的访问变化能够按预期执行。Microsoft 的文档指出，动态成员组本身还受许可要求和规则属性安全性约束。

## 过渡期结束后需持续验证

Microsoft 的最终提醒设定了明确的退役日期，但企业完成规则替换后仍需验证实际成员列表和访问结果。仅仅删除 MemberOf 条件并不保证权限配置正确；管理员需要检查替代规则是否覆盖原有业务逻辑。若企业未在11月3日前完成迁移，现有成员数据可能停留在旧状态，造成访问和许可管理风险。
<<<CDB_EN>>>
# Microsoft Retires the Entra ID MemberOf Rule Operator on November 3, Warning Administrators to Update Configurations

Microsoft has issued a final reminder that the MemberOf rule operator in Microsoft Entra ID will be retired on November 3, 2026. Dynamic groups, dynamic administrative units and entitlement-management auto-assignment policies that rely on the operator will stop processing membership or assignment changes. Organizations that do not update their configurations may leave users without required access or licenses, while former employees could retain permissions that should have been removed.

## Retirement takes effect on November 3

Microsoft’s Message Center notice says the public-preview MemberOf operator will be retired on November 3. The company said it had observed that the feature could affect the scale and reliability of dynamic membership processing across a tenant, even when only one MemberOf rule was present. Microsoft therefore decided to end the preview rather than recommend the functionality for production use.

The deadline applies to configurations that use the operator in the supported Entra ID features identified by Microsoft. Administrators should not assume that existing rules will continue to update after the retirement date.

## Dynamic group membership updates will stop

Microsoft said dynamic groups using MemberOf will stop processing membership changes. Dynamic administrative units that rely on the operator will stop updating membership and administrative scope. Entitlement Management auto-assignment policies using MemberOf will also stop processing assignment updates.

Existing membership and assignment data will remain in its last known state. That means the data will not necessarily disappear, but it may become outdated as employees join, leave or change roles within an organization.

## Stale permissions can create security risks

If dynamic membership stops updating, new employees may not receive the access or licenses they need. Former employees may retain access or licenses that should have been removed. Conditional Access policies that rely on affected groups may evaluate outdated membership information. Microsoft also warned that Teams, SharePoint and other applications depending on dynamic groups could receive stale membership data.

These risks make the retirement more than a technical change to a rule operator. The affected configurations can influence identity management, application access and licensing decisions across an organization.

## Administrators must replace rules or assign membership manually

Microsoft recommends exporting dynamic membership groups from the Entra admin center and identifying rules that contain MemberOf. Where possible, administrators should replace the operator with supported rule operators. If no supported dynamic alternative exists, Microsoft recommends converting the group to assigned membership.

The company also advises administrators to review dynamic administrative units and entitlement-management auto-assignment policies. After making changes, they should validate membership results, administrative scope and access-package assignments. Groups or administrative units that are no longer needed should be removed.

## The impact extends beyond one feature

MemberOf rules can be used in configurations that affect access control, licensing and administrative scope. Organizations should review Conditional Access policies and other systems that rely on dynamic group membership. They should also verify that new employees receive the correct permissions and that former employees lose access when required.

Microsoft’s documentation separately notes that dynamic membership groups have licensing requirements and that the security of membership depends on who can modify the attributes used in rules. Those considerations remain relevant when organizations redesign their configurations.

## Validation remains necessary after migration

The retirement date is fixed, but replacing a rule does not automatically guarantee that the resulting access configuration is correct. Administrators need to verify that the new rule or assigned-membership process preserves the organization’s intended business logic.

If a company has not completed the migration by November 3, affected membership and assignment information may remain frozen at its last known state. The practical risk is that identity, access and licensing systems may no longer reflect employees’ current roles. Microsoft’s final reminder is therefore a deadline for both technical replacement and validation.
<<<CDB_META>>>
{
  "title_zh": "Microsoft Entra ID的MemberOf规则运算符于11月3日退役，企业需检查动态组配置",
  "title_en": "Microsoft Retires the Entra ID MemberOf Rule Operator on November 3, Warning Administrators to Update Configurations",
  "section": "科技",
  "sources": [
    {"publisher":"Microsoft","title":"MC1488834 - Microsoft Entra ID: Final reminder to replace MemberOf rule operator configurations by November 3, 2026","url":"https://mc.merill.net/message/MC1488834"},
    {"publisher":"Microsoft Learn","title":"Manage rules for dynamic membership groups in Microsoft Entra ID","url":"https://learn.microsoft.com/en-us/entra/identity/users/groups-dynamic-membership"},
    {"publisher":"Neowin","title":"Microsoft issues final warning and guidance on Entra ID MemberOf retirement","url":"https://www.neowin.net/news/microsoft-issues-final-warning-and-guidance-on-entra-id-memberof-retirement/"}
  ],
  "numbers_check": [
    {"数字":"2026年11月3日","出处":"Microsoft Message Center MC1488834：MemberOf规则运算符退役日期"},
    {"数字":"15,000个","出处":"Microsoft Learn：单个租户可创建的动态成员组上限"}
  ],
  "uncertain": ["Microsoft原始Message Center通知通过公开归档镜像读取；正式操作应以管理员租户中的Message Center通知为准。"]
}
<<<CDB_DONE>>>