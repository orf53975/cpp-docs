---
title: "CSession::Open | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.technology: ["cpp-data"]
ms.topic: "reference"
f1_keywords: ["ATL::CSession::Open", "CSession::Open", "CSession.Open", "ATL.CSession.Open"]
dev_langs: ["C++"]
helpviewer_keywords: ["Open method"]
ms.assetid: c2050c2c-9817-4857-be49-189f346968f6
author: "mikeblome"
ms.author: "mblome"
ms.workload: ["cplusplus", "data-storage"]
---
# CSession::Open
Opens a new session for the data source object.  
  
## Syntax  
  
```cpp
HRESULT Open(const CDataSource& ds,  
   DBPROPSET *pPropSet = NULL,  
   ULONG ulPropSets = 0) throw();  
```  
  
#### Parameters  
 `ds`  
 [in] The data source for which the session is to be opened.  
  
 *pPropSet*  
 [in] A pointer to an array of [DBPROPSET](https://msdn.microsoft.com/en-us/library/ms714367.aspx) structures containing properties and values to be set. See [Property Sets and Property Groups](https://msdn.microsoft.com/en-us/library/ms713696.aspx) in the *OLE DB Programmer's Reference* in the Windows SDK.  
  
 `ulPropSets`  
 [in] The number of [DBPROPSET](https://msdn.microsoft.com/en-us/library/ms714367.aspx) structures passed in the *pPropSet* argument.  
  
## Return Value  
 A standard `HRESULT`.  
  
## Remarks  
 You must open the data source object using [CDataSource::Open](../../data/oledb/cdatasource-open.md) before passing it to `CSession::Open`.  
  
## Requirements  
 **Header:** atldbcli.h  
  
## See Also  
 [CSession Class](../../data/oledb/csession-class.md)