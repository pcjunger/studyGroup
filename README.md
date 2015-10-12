Grupo de Estudo Mozilla
============

Bem vindo ao [Mozilla Science Lab](https://www.mozillascience.org/)'s Projeto grupo de estudo! A partir daqui, iremos disponibilizar tudo que você precisa para começar o seu
próprio grupo de estudo.

### Pera ai, o que é um 'Grupo de Estudo Mozilla'?

Grupos de estudo Mozilla são divertidos, encontros informais com seus amigos e colegas ao redor de instituições locais e cidades para compatilhar habilidades,
histórias e ideias sobre o uso de programação em pesquisa. O objetivo é criar um ambiente
amigável e sem pressão onde as pessoas podem compartilhar seus trabalhos, pedir ajuda
para resolver problemas de programação e aprender e trabalhar junto com seus parceiros.

## Para Participantes

Bem-vindos ao Grupo de Estudos Mozilla! Algumas coisas que você precisa fazer & saber agora que vocês está aqui:

 - **Assista esse repo:** no topo direito desta página, existe um botão 'Watch'; clique nele para acompanhar esse repositório. Agora você receberá notificações de novas discussões do grupo por e-mail; se você não quer receber e-mails, mas gostaria de receber mensagens de alerta apenas no GitHub, mude as configurações em 'Settings' –> 'Notification Center' (Acesse configurações clicando na pequena roldana que encontra-se na barra lateral à direita).
 - **Check out the issue tracker:** clique em 'issues' na barra lateral à direita; aqui é onde todas as conversas desse grupo de estudos acontencem. Utilize este espaço para fazer perguntas, requerer eventos, fazer sugestões, ou apenas dar um alô.
 - **Leia o código de conduta:** esse Grupo de Estudos é para todos - nós cumprimos uma [série de regras](https://www.mozillascience.org/code-of-conduct/) que requer que todos seham tratados com respeito. Ajude-nos a construir um espaço onde sintam-se bemvindos, e todos teremos um tempo melhor juntos!
 - **Seja adicionado ao nosso website:** Se você quer aparecer como colaborador no nosso website sob a seção 'Who we Are' (Quem nós Somos), dê uma olhada em `_data/members.yml`; envie-nos um pull request com a sua entrada, ou abra um novo 'issue' e nós faremos isso por você.

## For Organizers

### It's Broken, I Need Help

If anything in these instructions doesn't work or doesn't make sense, open an issue [here](https://github.com/mozillascience/studyGroup/issues) or email sciencelab@mozillafoundation.org.

### Check out the Handbook

The instructions below will help you set up the online tools for your Mozilla Study Group - but if you're looking for organziation strategies, event plans and lesson ideas, check out the [Mozilla Study Group Handbook](https://mozillascience.github.io/studyGroupHandbook/)!

## How to Set Up Your Own Mozilla Study Group Website

Everything you need to set up your own Mozilla Study Group website for organizing events is right here - follow the following steps and you'll be up and running soon, and if you have trouble, [open an issue](https://github.com/mozillascience/studyGroup/issues) and we'll help you out!

 1. **Make yourself an account on GitHub.** The free one is just fine.
 2. **Fork this repository.** Up in the top right corner of this page, there's a button that says 'Fork'; press it! This makes your very own copy of all this stuff in your space on GitHub; when the copy is done, GitHub will automatically take you there.
 3. **Turn on the Issue Tracker.** An issue tracker is a message board GitHub sets up for every repository; you'll use it to post information about your event and talk to your participants. To turn it on: 
   - click on 'Settings' in the right sidebar of your repo;
   - click the checkbox beside 'Issues'; 
   - head back to your repo by clicking on the big `studyGroup` at the top of the page.
 4. **Edit the `_config.yml` file** in your new repository:
   - click on `_config.yml`;
   - click on the little pencil near the top right;
   - follow the instructions in the file on how to edit it; 
   - when you're done, press the green 'Commit Changes' button at the bottom of the page.

That's it, you're done! You can see your new website at `https://yourUserName.github.io/studyGroup/`, where `yourUserName` is the user name you signed up for GitHub with. If this is your first time making a webpage on GitHub, it might take 30 minutes for things to percolate through their computers - don't worry, it's all good, check back later and your website should be up and running.

### Optional: Setting up a Google Calendar for your Study Group

If you'd like to offer your community a calendar of events they can import into their own calendars, try using a Google Calendar. To set up, make a new google account, and update the variables in `_config.yml` under the heading 'Setup Google Calendar'.

You can add events to your calendar by hand, but if you'd like to manage it automatically, there's a script to do so in `scripts/updateCalendar.py`; instructions for use are at the top of that file.

## How to Launch a New Event

When you're ready to list a new event for your Study Group, follow these steps, or [watch this video](https://youtu.be/abglQgEIccw) where we walk you through event listing.

 1. **Make a new Issue to describe your event.** 
   - Click on 'Issues' over on the right sidebar of your repo, 
   - click the green 'New Issue' button near the top right. 
   - You'll then see a form where you can give your event a title and a description - fill these out with all the relevant information:
     - Where will your event be? Include a link to a map.
     - When will it be? Date and time.
     - Should people do anything to prepare beforehand (install any dependencies, set something up?)
 2. **Go to the `_posts` directory**. It'll be at `https://github.com/yourUserName/studyGroup/tree/gh-pages/_posts` - or you can click on `_posts` in your repo.
 3. **Make a new file** by clicking on the `+` sign beside `_posts/` Name it like the following:

    ```
    YYYY-MM-DD-word.markdown
    ```

    where `YYYY-MM-DD` is the date of your event, and `word` is anything you want.
 4. **Cut and paste the following into your new file:**
 
    ```
    ---
    title: Study Group Meetup
    text: a one sentence description of your event
    location: Hacky Hour Stadium
    link: https://github.com/yourUserName/studyGroup/issues/1234
    date: 2016-01-04
    startTime: '15:00'
    endTime: '16:00'
    ---
    ```

    Change all the fields to describe your event; make sure the `link` is the address of the issue you created When you're done, click 'Commit Changes' at the bottom.

That's it! Your event is now listed on your webpage, and there's a discussion thread where people can ask questions and discuss the details. Events will be automatically removed from the schedule on the webpage when they're more than a week in the past - but the issue you created will always be there as a record of what you've done.

> **Event Listing Gotchas:** here are a few things to look out for when listing an event:
>  - Did you remember to include the `---` above and below? The website builder needs those.
>  - Can't find the issue tracker? Remember to turn it on under the 'Settings' menu on the right.
>  - The seven fields need to be on exactly one line each; some text editors will insert line breaks into lines that are too long; remove these if so.

## How to Stay in Touch With Your Members

Now that you're all set up, GitHub provides several ways to stay in touch with the people involved in your Study Group.

  - **Ask users to Watch your repo.** Make sure all your users click 'Watch' at the top of your repository. This way, they'll be automatically notified of all the events you post in your issue tracker. 
  - **Use the Issue Tracker.** The Issue Tracker is your public message board to make announcements, ask questions and start conversations with your members. You can find yours at `https://github.com/yourUserName/studyGroup/issues`.
  - **Use the Mozilla Science Forum** to chat with study groups worldwide. Find the [forum here](https://forum.mozillascience.org/category/events/study-groups); use this to share your stories, ask questions to the wider community, and find out who's out there.

## Feature Your Community in the 'Who We Are' Section

Your website includes a gallery of participants in your Study Group; adding people here is a great way to show off your community and highlight your new friends and colleagues. To add someone to the list, edit the `_data/members.yml` file by adding the following section for them:

```
- name: their human name
  affiliation: school, lab, department, business....
  github: their GitHub handle
  interests:
    - list one to three
    - different interests
```
