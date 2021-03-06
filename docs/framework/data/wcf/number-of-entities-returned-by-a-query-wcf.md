---
title: "How to: Determine the Number of Entities Returned by a Query (WCF Data Services)"
ms.date: "03/30/2017"
dev_langs: 
  - "csharp"
  - "vb"
helpviewer_keywords: 
  - "WCF Data Services, row count"
ms.assetid: 03d41a82-df95-40ac-8439-a6c327d37ba8
---
# How to: Determine the Number of Entities Returned by a Query (WCF Data Services)
With [!INCLUDE[ssAstoria](../../../../includes/ssastoria-md.md)], you can determine the number of entities that are in the entity set specified by a query URI. This count can be included either along with the query result or as an integer value. For more information, see [Querying the Data Service](querying-the-data-service-wcf-data-services.md).  
  
 The example in this topic uses the Northwind sample data service and autogenerated client data service classes. This service and the client data classes are created when you complete the [WCF Data Services quickstart](quickstart-wcf-data-services.md).  
  
## Example  
 This example executes a query after calling the <xref:System.Data.Services.Client.DataServiceQuery%601.IncludeTotalCount%2A> method. The <xref:System.Data.Services.Client.QueryOperationResponse%601.TotalCount%2A> property returns the number of entities in the `Customers` entity set.  
  
 [!code-csharp[Astoria Northwind Client#CountAllCustomers](../../../../samples/snippets/csharp/VS_Snippets_Misc/astoria_northwind_client/cs/source.cs#countallcustomers)]
 [!code-vb[Astoria Northwind Client#CountAllCustomers](../../../../samples/snippets/visualbasic/VS_Snippets_Misc/astoria_northwind_client/vb/source.vb#countallcustomers)]  
  
## Example  
 This example calls the <xref:System.Linq.Enumerable.Count%2A> method to return only an integer value that is the number of entities in the `Customers` entity set.  
  
 [!code-csharp[Astoria Northwind Client#CountAllCustomersValueOnly](../../../../samples/snippets/csharp/VS_Snippets_Misc/astoria_northwind_client/cs/source.cs#countallcustomersvalueonly)]
 [!code-vb[Astoria Northwind Client#CountAllCustomersValueOnly](../../../../samples/snippets/visualbasic/VS_Snippets_Misc/astoria_northwind_client/vb/source.vb#countallcustomersvalueonly)]  
  
## See also

- [Querying the Data Service](querying-the-data-service-wcf-data-services.md)
