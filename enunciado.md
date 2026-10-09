# Enunciado: exercício prático

## Objetivo

O exercício tem como objetivo dar a conhecer algumas das tecnologias utilizadas no Departamento de Informática, através da evolução de um website simples para um evento, desenvolvido em Vue.js.

Não é necessária experiência prévia em programação.

## Como funciona

- **Duração estimada:** 1 a 2 horas.
- **Não é esperado que todas as tarefas sejam concluídas.** As tarefas estão organizadas por dificuldade crescente e basta realizar as que conseguir. É preferível fazer menos tarefas e compreendê-las bem.
- **É permitido o uso de ferramentas de IA** (é recomendado), desde que seja capaz de explicar o que escreveu. Na entrevista, será pedido que explique parte das alterações feitas.
- **Antes de começar**, siga as instruções de instalação e execução do [`README.md`](README.md).

## Tarefas

Sugerimos que siga a ordem apresentada.

### Nível 1: Introdutório

**1. Alterar as cores do website.**
Modificar as cores da página, de modo a que o resultado seja visivelmente diferente do original.
*Ficheiro relevante:* `src/style.css`

**2. Adicionar uma atividade ao horário.**
Acrescentar uma nova atividade à lista, de modo a que apareça na página.
*Ficheiro relevante:* `src/data/activities.js`

### Nível 2: Intermédio

**3. Acrescentar local e data aos cartões do horário.**
Cada cartão deve passar a mostrar o local e a data da respetiva atividade, para todas as atividades da lista.
*Ficheiros relevantes:* `src/data/activities.js` e `src/components/ScheduleList.vue`

**4. Acrescentar um campo ao formulário de inscrição.**
Adicionar um novo campo ao formulário (por exemplo, curso ou ano), que deve ser tratado da mesma forma que os restantes campos.
*Ficheiro relevante:* `src/components/SignUpForm.vue`

### Nível 3: Avançado

**5. Impedir inscrições com o mesmo email.**
Se uma pessoa tentar inscrever-se com um email já utilizado, a inscrição não deve ser aceite e deve ser apresentada uma mensagem clara ao utilizador.
*Ficheiro relevante:* `src/components/SignUpForm.vue`

**6. Criar um novo componente.**
Criar um componente novo (por exemplo, `SpeakersSection.vue`, com a lista de oradores do evento) e incluí-lo na página.
*Ficheiros relevantes:* `src/components/` e `src/App.vue`

## Entrega

A entrega deve ser feita **até ao final do dia anterior à data da entrevista (23h59)**, por email para **informatica.sbe.ist@gmail.com**.

1. Eliminar a pasta `node_modules` do projeto, caso exista.
2. Comprimir a pasta do projeto num ficheiro ZIP, com o nome `Nome_Apelido.zip`.
3. Enviar o ficheiro, indicando no email o nome, o curso e o ano, e uma descrição breve do que foi feito.

## Entrevista

A entrevista será uma conversa informal sobre o exercício e a sua candidatura. Sugerimos que se prepare para explicar:

- o que fez e como o fez;
- as dificuldades encontradas e como as resolveu;
- o que aprendeu com o exercício.

O que será avaliado é o raciocínio e o interesse demonstrados, não a perfeição do resultado.