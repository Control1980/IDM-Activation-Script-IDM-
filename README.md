IDM Activation Script IDM 激活脚本
Activation:

    This script applies the registry lock method to activate the Internet Download Manager (IDM).
    此脚本应用注册表锁定方法来激活 Internet 下载管理器 (IDM)。

    This method requires Internet at the time of activation.
    此方法在激活时需要互联网。

    IDM updates can be installed directly without having to activate again.
    IDM更新可以直接安装，无需再次激活。

    After the activation, if in some cases, the IDM starts to show an activation nag screen, then just run the activation option again.
    激活后，如果在某些情况下，IDM 开始显示激活导航屏幕，则只需再次运行激活选项即可。

Reset IDM Activation / Trial: 重置 IDM 激活/试用：

    The Internet Download Manager provides 30 days trial period, you can use this script to reset this Activation / Trial period whenever you want.
    Internet Download Manager 提供 30 天试用期，您可以随时使用此脚本重置此激活/试用期。

    This option also can be used to restore status if in case the IDM reports a fake serial key and other similar errors.
    如果 IDM 报告伪造的序列密钥和其他类似错误，此选项还可用于恢复状态。

OS requirement: Windows 7, 8, 8.1, 10 & 11
操作系统要求：Windows 7、8、8.1、10 和 11
How to use it? 如何使用它？
PowerShell

On Windows 10/11, right-click on the windows start menu and select PowerShell or Terminal.
在 Windows 10/11 上，右键单击 Windows 开始菜单，然后选择 PowerShell 或终端。

Copy-paste the below code and press enter:
复制粘贴以下代码并按 Enter：

iex(irm is.gd/idm_reset)

or

iwr -useb https://raw.githubusercontent.com/lstprjct/IDM-Activation-Script/main/IAS.ps1 | iex

You will see the activation options, and follow onscreen instructions.
您将看到激活选项，并按照屏幕上的说明进行操作。

That's all.

    Project is supported only for Windows 7/8/8.1/10/11 and their Server equivalent.
    仅 Windows 7/8/8.1/10/11 及其等效服务器支持项目。

- Advanced Info: - 高级信息：

    To add a custom name in IDM license info, edit line number 5 in the script file.
    要在 IDM 许可证信息中添加自定义名称，请编辑脚本文件中的第 5 行。
    For activation in unattended mode, run the script with /act parameter.
    要在无人值守模式下激活，请使用 /act 参数运行脚本。
    For reset in unattended mode, run the script with /res parameter.
    要在无人值守模式下重置，请使用 /res 参数运行脚本。
    To enable silent mode with the above two methods, run the script with /s parameter.
    要使用上述两种方法启用静默模式，请使用 /s 参数运行脚本。

Possible accepted values, 可能接受的值，

"IAS_xxxxxxxx.cmd" /act "IAS_xxxxxxxx.cmd" /res "IAS_xxxxxxxx.cmd" /act /s "IAS_xxxxxxxx.cmd" /res /s
- Troubleshooting steps: - 故障排除步骤：

    If any other activator was used to activate IDM previously then make sure to properly uninstall it with that same activator (if there is an option), this is especially important if any registry/firewall block method was used.
    如果之前使用任何其他激活器激活 IDM，请确保使用相同的激活器正确卸载它（如果有选项），如果使用任何注册表/防火墙阻止方法，这一点尤其重要。

    Uninstall the IDM from the control panel.
    从控制面板卸载 IDM。

    Make sure the latest original IDM setup is used for the installation, you can download it from https://www.internetdownloadmanager.com/download.html
    确保使用最新的原始IDM安装程序进行安装，您可以从 https://www.internetdownloadmanager.com/download.html 下载它

    Now install the IDM and use the activate option in this script if failed then,
    现在安装 IDM 并使用此脚本中的激活选项（如果失败），

        Disable the windows firewall with the script option, this helps in case of leftover entries of previously used activator (some file patch method also creates firewall entries).
        使用脚本选项禁用 Windows 防火墙，这有助于防止以前使用的激活器的剩余条目（某些文件修补方法也会创建防火墙条目）。

        Some security programs may block this script, this is false-positive, as long as you downloaded the file from the original post (mentioned below on this page), temporary suspend Antivirus real-time protection, or exclude the downloaded file/extracted folder from scanning.
        某些安全程序可能会阻止此脚本，这是误报，只要您从原始帖子（本页下面提到的）中下载该文件，暂时暂停防病毒实时保护，或从其中排除下载的文件/解压文件夹即可扫描。

        If you are still facing any issues, please contact me (mentioned below on this page).
        如果您仍然遇到任何问题，请与我联系（本页下面提到）。

Credits:

@Dukun Cabul - Original researcher of this IDM trial reset and activation logic, made an Autoit tool for these methods, IDM-AIO_2020_Final nsaneforums.com/topic/371047--/?do=findComment&comment=1632062
@Dukun Cabul - 此 IDM 试验重置和激活逻辑的原始研究员，为这些方法制作了 Autoit 工具，IDM-AIO_2020_Final nsaneforums.com/topic/371047--/?do=findComment&comment=1632062

@WindowsAddict - Ported the above Autoit tool to a batch script
@WindowsAddict - 将上述 Autoit 工具移植到批处理脚本中

@AveYo aka @BAU - Snippet to set registry ownership and permission recursively pastebin.com/XTPt0JSC
@AveYo 又名 @BAU - 用于递归设置注册表所有权和权限的代码片段pastebin.com/XTPt0JSC

@abbodi1406 - Awesome batch script tricks and help
@abbodi1406 - 很棒的批处理脚本技巧和帮助

@dbenham - Set buffer height independently of window height stackoverflow.com/a/13351373
@dbenham - 设置缓冲区高度与窗口高度无关 stackoverflow.com/a/13351373

@ModByPiash (Me) - Add and fix some missing features.
@ModByPiash (Me) - 添加并修复一些缺失的功能。

@vavavr00m - Changed set name to prompt for a name
@vavavr00m - 更改了集名称以提示输入名称
IDM Activation Script IDM 激活脚本
Telegram: https://t.me/ModByPiash 电报： https://t.me/ModByPiash

Forum: https://www.nsaneforums.com/topic/371047--/?do=findComment^&comment=1578647 论坛： https://www.nsaneforums.com/topic/371047--/?do=findComment^&comment=1578647 
