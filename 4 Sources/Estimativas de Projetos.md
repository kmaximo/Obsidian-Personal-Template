
up:: 
tags:: 

# Estimativas de Projetos

# Melhore suas estimativas de projetos e entregas com a técnica PERT

Tempo é um recurso valioso em qualquer projeto ou negócio, e estimar corretamente o tempo necessário para concluir uma tarefa é fundamental para garantir que os prazos sejam cumpridos e as expectativas dos clientes sejam atendidas. No entanto, muitas vezes pode ser desafiador determinar com precisão quanto tempo uma tarefa levará, especialmente quando há muitas variáveis envolvidas.

No livro O codificador limpo da série de **Robert C. Martin**, existe um capitulo inteiro sobre estimativa (capitulo 10), apresentando a **PERT** (Program Evaluation and Review Technique).

PERT é uma técnica de gerenciamento de projetos que ajuda a estimar o tempo necessário para completar uma tarefa ou projeto, A técnica usa uma abordagem probabilística para estimar o tempo de conclusão de uma tarefa. Em vez de fornecer uma única estimativa de tempo, a PERT usa três valores:

**O:** Estimativa Otimista. Este número é altamente otimista. Ou seja você só consegue completar a tarefa nessa velocidade se tudo der certo.

**N:** Estimativa Nominal: Esta é a estimativa com a maior chance de sucesso.

**P:** Estimativa Pessimista: Este numero é altamente pessimista. Inclui tudo que pode dar errado ao executar essa tarefa (exceto furacões, guerra nuclear, buracos negros e outras catástrofes).

Podemos descrever a distribuição da probabilidade:

R = (O+4N+P)/6

Estimativa de tempo = (Valor otimista + (4 x valor mais provável) + valor pessimista) / 6

Para exemplicar:

Valor otimista: 1 dia.  
Valor mais provável: 3 dias.  
Valor pessimista: 6 dias.

podemos usar diferentes unidades de tempo (horas, dias, semanas, meses, etc.).

R = (1 + (4 x 3) + 6) / 6  
R = (1 + 12 + 6) / 6  
R = 19 / 6  
R = 3,1666666667

Portanto, a estimativa mais realista para a conclusão da tarefa é de aproximadamente 3,17 (**dias**).