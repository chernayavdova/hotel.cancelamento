# Reservas Canceladas Dashboard
Análise no excel de um dashboard com os dados de reservas canceladas.


### Sumário

- Análise com o objetivo de saber o motivo dos cancelamentos.

### Motivo da Análise

- Saber os meses com mais reservas/cancelamentos, tipos de hóspedes que mais cancelam, tipo de hotel que tem mais cancelamento.

### Metas 

- Diminuir a taxa de cancelamento.

### Dataset

![Captura de tela 2024-04-17 141449](https://github.com/chernayavdova/hotel.cancelamento/assets/86575159/fb0075c4-ece1-4374-9d76-825d9fa6c4f7)

- O dataset contém as seguintes informações:
  - 32 colunas e 119.391 linhas
 
### Metodologia
  - Após a limpeza dos dados, fiz a tradução das informações e também retirei as colunas que não preciso para a análise. Restou 12 colunas originais e 2 colunas criadas.
 
    ![Captura de tela 2024-04-17 142305](https://github.com/chernayavdova/hotel.cancelamento/assets/86575159/f25dd542-9fb2-4883-8a5b-02f1539aba5d)

  - As colunas criadas são: room_type e guest_type
      - Coluna room_type: utilizei a função "SE" para cruzar os dados das colunas "reserved_room_type" e "assigned_room_type" para saber se o quarto reservado foi o quarto recebido na hora do check-in. Caso tenha sido o reservado, o "room_type" retorna "Desejado", caso contrário, "Não Desejado".
      - ![Captura de tela 2024-04-17 143546](https://github.com/chernayavdova/hotel.cancelamento/assets/86575159/240f974a-28e5-4b61-a396-b494646879c7)

      - Coluna "guest_type": também utilizei a função "SE" e "E" para cruzar os dados das colunas "adults", "children" e "babies" para saber se o quarto tinha sido reservado por um casal, solteiro ou familia.
      - ![Captura de tela 2024-04-17 143555](https://github.com/chernayavdova/hotel.cancelamento/assets/86575159/195a5af1-c1ea-4d71-9bef-1db284cd8f83)

### Dashboard

![Captura de tela 2024-04-17 143326](https://github.com/chernayavdova/hotel.cancelamento/assets/86575159/308658b8-6076-42dd-9a6c-33eeba593d5c)

- Podemos ver no grafico "Total de Hospedes por Tipo e Total de Cancelamentos", que a maioria das reservas foram feitas por casais, consequentemente a maioria dos cancelamentos também.
- No gárfico "Tipo de Quarto e Cancelamentos" vemos que 88% dos hóspedes tiveram o quarto desejado, mas, apesar disso o número de cancelamentos é alto. Em comparação, apenas 5% dos hóspedes que reservaram um quarto e na hora do check-in não receberam o quarto desejado, cancelaram.
- Hoteis na cidade são os mais procurados, com 39.270 reservas a mais do que os Resorts.
- 42% das reservas nos Hoteis na Cidade são canceladas, embora as reservas sejam menores nos resorts, a taxa de cancelamento também é, chegando a 28%.
- Os meses com a menos cancelamentos são: Novembro, Dezembro e Janeiro. Os com o maior número de cancelamento são: Agosto, Julho e Maio.

### Conclusão
Vimos que o número de reservas canceladas é bem alto com casais e mesmo quando o quarto desejado esta disponível. Vimos também que os Hoteis que ficam na cidade sofrem mais com os cancelamentos do que os Resorts.


 

