---
title: "IDebugDynamicFieldCOMPlus::GetTypeFromTypeDef | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "GetTypeFromTypeDef"
  - "IDebugDynamicFieldCOMPlus::GetTypeFromTypeDef"
ms.assetid: 7f6cd3d3-f4da-4893-be91-8dd104be8010
caps.latest.revision: 8
ms.author: "gregvanl"
manager: "ghogen"
translation.priority.mt: 
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
# IDebugDynamicFieldCOMPlus::GetTypeFromTypeDef
Retrieves a type given its token.  
  
## Syntax  
  
```cpp  
HRESULT GetTypeFromTypeDef(  
   ULONG32       ulAppDomainID,  
   GUID          guidModule,  
   _mdToken      tokClass,  
   IDebugField** ppType  
);  
```  
  
```csharp  
int GetTypeFromTypeDef(  
   uint            ulAppDomainID,  
   Guid            guidModule,  
   int             tokClass,  
   out IDebugField ppType  
);  
```  
  
#### Parameters  
 `ulAppDomainID`  
 [in] Identifier of the application domain.  
  
 `guidModule`  
 [in] Unique identifier of the module.  
  
 `tokClass`  
 [in] Token that represents the type.  
  
 `ppType`  
 [out] Returns an [IDebugField](../../../extensibility/debugger/reference/idebugfield.md) object that contains the type.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## See Also  
 [IDebugDynamicFieldCOMPlus](../../../extensibility/debugger/reference/idebugdynamicfieldcomplus.md)