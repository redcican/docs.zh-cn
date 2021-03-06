---
title: 如何：读取文本文件中的内容 - C# 编程指南
ms.custom: seodec18
ms.date: 07/20/2015
f1_keywords:
- StreamReader.ReadToEnd
helpviewer_keywords:
- text files, writing to
- reading text files
- reading data, text files
- text files, reading
ms.assetid: 92246c5b-e819-4eea-9370-1a9460e12de3
ms.openlocfilehash: 560453a81124a3ee52a2ffd794ddac026c7394a5
ms.sourcegitcommit: 40364ded04fa6cdcb2b6beca7f68412e2e12f633
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2019
ms.locfileid: "56978015"
---
# <a name="how-to-read-from-a-text-file-c-programming-guide"></a>如何：读取文本文件中的内容（C# 编程指南）
此示例通过使用 <xref:System.IO.File?displayProperty=nameWithType> 类的 <xref:System.IO.File.ReadAllText%2A> 和 <xref:System.IO.File.ReadAllLines%2A> 静态方法来确定文本文件的内容。  
  
 有关使用 <xref:System.IO.StreamReader> 的示例，请参阅[操作说明：一次一行地读取文本文件](../../../csharp/programming-guide/file-system/how-to-read-a-text-file-one-line-at-a-time.md)。  
  
> [!NOTE]
>  此示例所用的文件是在主题[操作说明：写入到文本文件](../../../csharp/programming-guide/file-system/how-to-write-to-a-text-file.md)中创建。  
  
## <a name="example"></a>示例  
 [!code-csharp[csFilesandFolders#4](~/samples/snippets/csharp/VS_Snippets_VBCSharp/csFilesAndFolders/CS/FileIteration.cs#4)]  
  
## <a name="compiling-the-code"></a>编译代码  
 将代码复制并粘贴到 C# 控制台应用程序。  
  
 如果不使用[操作说明：写入到文本文件](../../../csharp/programming-guide/file-system/how-to-write-to-a-text-file.md)中的文本文件，请将 `ReadAllText` 和 `ReadAllLines` 的参数替换为计算机上的适当路径和文件名。  
  
## <a name="robust-programming"></a>可靠编程  
 以下情况可能会导致异常：  
  
-   不存在该文件，或者指定位置不存在该文件。 检查文件名的路径和拼写。  
  
## <a name="net-framework-security"></a>.NET Framework 安全性  
 不要依赖文件名来确定文件的内容。 例如，文件 `myFile.cs` 可能不是 C# 源文件。  
  
## <a name="see-also"></a>请参阅

- <xref:System.IO?displayProperty=nameWithType>
- [C# 编程指南](../../../csharp/programming-guide/index.md)
- [文件系统和注册表（C# 编程指南）](../../../csharp/programming-guide/file-system/index.md)
