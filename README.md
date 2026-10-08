# Semana da Bioengenharia (Vue + Vite)

Projeto base do exercício prático do Departamento de Informática. As tarefas a realizar encontram-se no ficheiro [`enunciado.md`](enunciado.md). Este documento explica como instalar e executar o projeto.

Não é necessário ter experiência prévia com Vue.js. Basta abrir os ficheiros que o enunciado mencionar.

---

## Pré-requisitos

1. **Node.js**, versão LTS: [nodejs.org](https://nodejs.org). Após a instalação, abrir um terminal e executar `node -v`. Se for apresentado um número de versão, a instalação está correta.
2. **Um editor de código.** Recomendamos o [Visual Studio Code](https://code.visualstudio.com).

## Instalação (apenas uma vez)

1. Se o projeto foi descarregado em ZIP, **extrair o conteúdo para uma pasta**. Não se deve trabalhar dentro do ficheiro ZIP.
2. No VS Code, abrir a pasta do projeto: **File → Open Folder**.
3. Abrir um terminal dentro do VS Code: **Terminal → New Terminal**. O terminal já fica posicionado na pasta do projeto.
4. Executar:

```
npm install
```

A instalação pode demorar alguns minutos.

## Executar o projeto

```
npm run dev
```

O terminal apresenta um endereço (normalmente `http://localhost:5173`). Abri-lo no browser. A página atualiza-se automaticamente sempre que um ficheiro é guardado (`Ctrl + S` ou `Cmd + S`).

Para parar o servidor, premir `Ctrl + C` no terminal.

## Estrutura do projeto

- `src/App.vue`: a página principal, que reúne os componentes (o nome e a data do evento definem-se aqui).
- `src/components/`: um ficheiro por secção (`HeroSection`, `ScheduleList`, `SignUpForm`).
- `src/data/activities.js`: o horário das atividades.
- `src/style.css`: estilos globais e cores (cada componente tem ainda o seu bloco `<style scoped>`).

Cada ficheiro `.vue` tem três partes:

- `<script setup>`: a lógica (JavaScript)
- `<template>`: a estrutura da página (HTML)
- `<style>`: o aspeto (CSS)

## Problemas comuns

**`npm` ou `node` "não é reconhecido como comando".**
Fechar e voltar a abrir o VS Code (ou o terminal) após instalar o Node.js. Se persistir, reiniciar o computador.

**No Windows: "a execução de scripts está desativada neste sistema".**
No terminal do VS Code, clicar na seta ao lado do botão `+` e escolher **Command Prompt**. Repetir o comando nesse terminal.

**A porta já está a ser utilizada.**
O Vite escolhe automaticamente outra porta. Utilizar o endereço que surge no terminal.

**A página aparece em branco ou com erro.**
Verificar a mensagem de erro no terminal e na consola do browser (`F12`). Normalmente indica o ficheiro e a linha onde está o problema.

**Qualquer outra dificuldade.**
Caso não seja possível resolver o problema, contactar o Departamento através de **informatica.sbe.ist@gmail.com**, incluindo a mensagem de erro, se existir.

## Entrega

As instruções de entrega estão no final do [`enunciado.md`](enunciado.md).