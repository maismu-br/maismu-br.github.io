# Cadastrar Item de Serviço Com Retenções Corretas

No cadastro de item quando formos cadastrar um serviço é necessário:

1. Deixar como um item de compra;
2. Caso tenha retenção de imposto (ISS, IR, CSLL, INSS, etc) - aqui normalmente tem;
3. Selecionar como serviço;
4. Preencher o código de serviço contratado com o código correto do serviço contratado;
5. Preencher o 4tax - lista de serviço com o código correto do serviço contratado, sem utilizar ponto; 
6. Preencher o 4tax - código atividade com o código correto do serviço contratado, sem utilizar ponto;
7. Preencher o 4tax - código tributação municipal com o código correto do serviço contratado, sem utilizar ponto.

Isso é para automatizar a ida da nota fiscal de serviço para o REINF, dentro do Orbit.

![1](/assets/images/item serviço 1.png#center)

- Para automatizar o cálculo da retenção dessa nota tem que criar a determinação fiscal para o serviço. Segue o caminho:

![2](/assets/images/item serviço 2.png#center)

- Ajustar o filtro;
- Na primeira linha está cadastrado os times de despesas que NÃO é para reter os impostos porque os fornecedores são optantes do Simples Nacional;
- Já na segunda linha são as despesas que precisam ter retenção sempre;
- Para abrir os detalhes precisa clicar duas vezes no número da linha.

![3](/assets/images/item serviço 3.png#center)

- Vai aparecer uma tela com todas as despesas cadastradas e para ter mais informações clica duas vezes no número da linha.

![4](/assets/images/item serviço 4.png#center)

- Vai abrir um tela mostrando as retenções autorizadas para serem feitas automaticamente e os percentuais de retenção para cada imposto.

![5](/assets/images/item serviço 5.png#center)

- Caso seja necessário alterar a alíquota de algum imposto:

![6](/assets/images/item serviço 6.png#center)

- Algo que NÃO PODE ACONTECER, não pode estão zerado a coluna Taxa:

![7](/assets/images/item serviço 7.png#center)

- Para criar um item novo é necessário preencher pela sequência do código, segue a descrição dos já criados, categoria normalmente é Nota Fiscal, tipo é bruto, valor base é normalmente 100%, tem que adicionar o código de retenção (tipo um CFOP de uma DANFE, mas para nota de serviço é outro código), Conta contábil e tipo de imposto. 
- Para adicionar a data e a taxa tem que clicar duas vezes no número da linha, coloca a data no efetivo desde de e a taxa SEM O % na taxa, exemplo 5,7% de retenção, preencher 5,7.

![8](/assets/images/item serviço 8.png#center)