---
title: .NET Framework 4 和 4.5 中添加的 CLR 承载接口
ms.date: 03/30/2017
helpviewer_keywords:
- hosting interfaces [.NET Framework], version 4
- .NET Framework 4, hosting interfaces
- interfaces [.NET Framework hosting], version 4
ms.assetid: f6af6116-f5b0-4bda-a276-fffdba70893d
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: e9086502968fb9046237e77b76b4038a9f32f4ef
ms.sourcegitcommit: c7f3e2e9d6ead6cc3acd0d66b10a251d0c66e59d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/09/2018
ms.locfileid: "44253086"
---
# <a name="clr-hosting-interfaces-added-in-the-net-framework-4-and-45"></a>.NET Framework 4 和 4.5 中添加的 CLR 承载接口
本部分介绍非托管接口的主机可用于将公共语言运行时 (CLR) 集成在[!INCLUDE[net_v40_long](../../../../includes/net-v40-long-md.md)]， [!INCLUDE[net_v45](../../../../includes/net-v45-md.md)]，并在其应用程序的更高版本。 这些接口提供的主机，若要配置和运行时加载到进程的方法。  
  
 从开始[!INCLUDE[net_v40_short](../../../../includes/net-v40-short-md.md)]、 所有托管接口具有以下特征：  
  
-   它们使用生命期管理 (`AddRef`并`Release`)，封装 （隐式上下文） 和`QueryInterface`从 com。  
  
-   存在不要使用 COM 类型，如`BSTR`， `SAFEARRAY`，或`VARIANT`。  
  
-   不没有使用任何单元模型、 聚合或注册表激活[CoCreateInstance 函数](https://go.microsoft.com/fwlink/?LinkId=142894)。  
  
## <a name="in-this-section"></a>本节内容  
 [ICLRAppDomainResourceMonitor 接口](../../../../docs/framework/unmanaged-api/hosting/iclrappdomainresourcemonitor-interface.md)  
 提供检查应用程序域的内存和 CPU 使用情况的方法。  
  
 [ICLRDomainManager 接口](../../../../docs/framework/unmanaged-api/hosting/iclrdomainmanager-interface.md)  
 使宿主能够指定将用于初始化默认应用程序域，并指定初始化属性的应用程序域管理器。  
  
 [ICLRGCManager2 接口](../../../../docs/framework/unmanaged-api/hosting/iclrgcmanager2-interface.md)  
 提供了[SetGCStartupLimitsEx](../../../../docs/framework/unmanaged-api/hosting/iclrgcmanager2-setgcstartuplimitsex-method.md)方法，使主机可以设置为值的垃圾回收段的大小和第 0 代垃圾回收系统的最大大小大于`DWORD`。  
  
 [ICLRMetaHost 接口](../../../../docs/framework/unmanaged-api/hosting/iclrmetahost-interface.md)  
 提供方法，返回特定版本的 CLR、 列出所有已安装的 Clr、 列出所有进程内运行时，返回激活接口，并发现用于编译的程序集的 CLR 版本。  
  
 [ICLRMetaHostPolicy 接口](../../../../docs/framework/unmanaged-api/hosting/iclrmetahostpolicy-interface.md)  
 提供了[GetRequestedRuntime](../../../../docs/framework/unmanaged-api/hosting/iclrmetahostpolicy-getrequestedruntime-method.md)提供 CLR 接口的方法基于策略条件、 托管程序集、 版本和配置文件。  
  
 [ICLRRuntimeInfo 接口](../../../../docs/framework/unmanaged-api/hosting/iclrruntimeinfo-interface.md)  
 提供返回有关特定运行时，包括版本、 目录和负载状态信息的方法。  
  
 [ICLRStrongName 接口](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-interface.md)  
 提供用于对程序集具有强名称签名基本全局静态函数。 所有[ICLRStrongName](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-interface.md)方法返回标准的 COM Hresult。  
  
 [ICLRStrongName2 接口](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname2-interface.md)  
 提供的功能来创建强名称使用 SHA-2 组的安全哈希算法 （SHA-256、 SHA-384 和 SHA-512）。  
  
 [ICLRTask2 接口](../../../../docs/framework/unmanaged-api/hosting/iclrtask2-interface.md)  
 提供的所有功能[ICLRTask 接口](../../../../docs/framework/unmanaged-api/hosting/iclrtask-interface.md); 此外，提供都了允许线程中止当前线程上延迟的方法。  
  
## <a name="related-sections"></a>相关章节  
 [弃用的 CLR 承接接口和组件类](../../../../docs/framework/unmanaged-api/hosting/deprecated-clr-hosting-interfaces-and-coclasses.md)  
 描述随.NET framework 1.0 和 1.1 版提供的托管接口。  
  
 [CLR Hosting 接口](../../../../docs/framework/unmanaged-api/hosting/clr-hosting-interfaces.md)  
 描述随.NET Framework 版本 2.0、 3.0 和 3.5 一起提供的托管接口。  
  
 [承载](../../../../docs/framework/unmanaged-api/hosting/index.md)  
 引入了在.NET Framework 中承载。
