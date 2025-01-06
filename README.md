Projeto para gerenciar uma equipe de vendas  dividido em :
- departamentos
- funcionário
- valor total de vendas
- filtro por departamenot
- filtro por data 

UML  Vendedor 
+-----------------------------------+
|             Vendedor              |
+-----------------------------------+
| - id: integer                     | 
| - nome: String                    |
| - email: String                   |
| - dataAniversario: Date           |
| - salario: double                 |      
+-----------------------------------+
| + addVenda(sr:VendaRecord): void |
| + removeVendas(sr:VendaRecord) : void |
| + totalVendido(initial: Date, final: Date): double |
+-----------------------------------+

UML Departamento 
+-----------------------------------+
|             Departamento          |
+-----------------------------------+
| - id: integer                     |
| - nome: String                    |
+-----------------------------------+
| + addVendedor(vendedor: Vendedor): void |
| + totalVenda(initial: Date, final: Date): double |
+-----------------------------------+

UML Venda
+-----------------------------------+
|           VendaRecord           |
+-----------------------------------+
| - id: integer                     |
| - date: Date                      |
| - amount: double                  |
| - status: VendaStatus             |
+-----------------------------------+

UML Status Venda
+------------------+
|    VendaStatus   |
+------------------+
| - PENDENTE: int  |
| - PAGO: int      |
| - CANCELADO: int |
+------------------+
