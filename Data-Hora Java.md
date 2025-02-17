
**Data:** 2025-02-15
**keyboards:** 
**links internos:** 
___
# Conceitos importantes:

- **Data-(hora) local**:
	ano-mês-dia-(hora) sem fuso horário
	(hora) opcional.

- **Data-hora global**:
	ano-mês-dia-hora com fuso horário.

- **Duração**:
	tempo decorrido entre duas data-horas.


![[Pasted image 20250217090449.png]]



# Quando usar?

- **Data-(hora) local**:
	Quando o momento exato não interessa a pessoas de outro fuso horário.
	Uso comum: Sistemas de região única, Excel.
		Data de nascimento: "15/06/2001"
		Data-hora da venda: "13/08/2022" às 15:32" (presumindo não interessar fuso horário)

- **Data-hora global**:
	Quando o momento exato interessa a pessoas de outro fuso horário.
	Uso comum: sistemas multi-região, web.
		Quando será o sorteio? "21/08/2022 às 20h (Horário de São Paulo)"
		Quando o comentário foi postado? "Há 17 minutos"
		Quando foi realizada a venda? "21/08/2022 às 15:32 (Horário de São Paulo)"
		Inicio e fim do evento? "21/08/2022 às 14h até 16h (Horário de São Paulo)"


# Timezone (fuso horário)

- **GMT - Greenwich Mean Time**.
	- Horário de Londres
	- Horário do padrão UTC - Coordinated Universal Time
	- também chamado de "Z" time, ou Zulu time.


- **Outros fuso horário são relativos ao GMT/UTC:**
	- São Paulo: GMT-3
	- Manaus: GMT-4
	- Portugal: GMT+1 


- **Muitas linguagens/Tecnologias usam nomes para as Timezones:**
	- "US/pacific"
	- "america/Sao_Paulo"
	- etc.


# Padrão ISO 8601

- **Data-(hora) local:**
	- 2022-07-21 2022-07-21T14:52 
	- 2022-07-22T14:52:09 
	- 2022-07-22T14:52:09.4073


- **Data hora global**:
	- 2022-07-23T14:52:09Z 
	- 2022-07-23T14:52:09.254935Z 
	- 2022-07-23T14:52:09-03:00


# Operações importantes com data-hora

- **Instanciação:**
	- (agora) -> Data-hora
	- Texto ISO 8601 -> Data-hora
	- Texto formato customizado -> Data-hora
	- dia, mês, ano, (Horario) - Data-hora local


- **Formatação**:
	- Data-hora -> Texto ISO 8601
	- Data-hora -> Texto customizado


- **Converter data-hora global para local**:
	- Data- hora global, Timezone (Sistema local) -> Data-hora local


- **Obter dados de uma data-hora local**.
	- Data-hora local -> dia, mês, ano, horário


-  **Cálculos com data-hora**:
	- Data-hora +/- tempo -> data hora
	- Date-hora 1, data-hora 2 -> Duração


# Principais tipos Java (versão8+)

- **Data-hora local**:
	- LocalDate
	- LocalDateTime

- **Data-hora global**:
	- Instant

- **Duração**:
	- Duration

- **Outros**:
	- Zoneld
	- ChronoUnit