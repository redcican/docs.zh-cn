---
title: （取模）（实体 SQL）
ms.date: 03/30/2017
ms.assetid: 243ddc4f-3c4e-41e1-a3ef-4ed39e36248b
ms.openlocfilehash: 543c35c56955fb0a9909fced23357444bc78197a
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54732591"
---
# <a name="modulo-entity-sql"></a>（取模）（实体 SQL）
返回两个表达式相除后的余数。  
  
## <a name="syntax"></a>语法  
  
```  
dividend % divisor  
```  
  
## <a name="arguments"></a>自变量  
 `dividend`  
 被除数的数值表达式。 `dividend` 为任何一种数值数据类型的任何有效表达式。  
  
 `divisor`  
 除数的数值表达式。 `divisor` 为任何一种数值数据类型的任何有效表达式。  
  
## <a name="result-types"></a>结果类型  
 Edm.Int32  
  
## <a name="example"></a>示例  
 以下 Entity SQL 查询使用 % 算数运算符以返回两个表达式相除后的余数。 此查询基于 AdventureWorks 销售模型。 若要编译并运行此查询，请执行下列步骤：  
  
1.  按照中的过程[如何：执行返回 StructuralType 结果的查询](../../../../../../docs/framework/data/adonet/ef/how-to-execute-a-query-that-returns-structuraltype-results.md)。  
  
2.  将以下查询作为参数传递给 `ExecuteStructuralTypeQuery` 方法：  
  
 [!code-csharp[DP EntityServices Concepts 2#MODULO](../../../../../../samples/snippets/csharp/VS_Snippets_Data/dp entityservices concepts 2/cs/entitysql.cs#modulo)]  
  
## <a name="see-also"></a>请参阅
- [实体 SQL 引用](../../../../../../docs/framework/data/adonet/ef/language-reference/entity-sql-reference.md)
