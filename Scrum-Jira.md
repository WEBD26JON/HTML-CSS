<!DOCTYPE html>
<html lang="sv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>{{ page.title }}</title>
    <link rel="stylesheet"
          href="{{ 'style.css' | relative_url }}">
</head>
<body>
    <main class="markdown-body">

# Scrum med Jira 

## 1. Переводим эльфийского на человеческй

Начнём с самого неприятного. Вот основные термины из документа, но без академических объяснений.

![Home](https://images.openai.com/static-rsc-4/L9Lvr1Q2k1KMoUFkpEkY1MHAJ78GKXZBRZhp1gHO3pBWQ_o3RCtqT6Q9pc5sTUc1WcLKRMVZUnTrM2n4_U7E40Y4zNmmkKmjDcGkv8HepXbTpEYKuqw_hrQxQaMlWQIO-w-nPIz3zt_vEqmZFdDuduKDyiktO6Ci57yyYoODjSgBLHq6K2w3kZMkejvm9GBs?purpose=fullsize)

Scrum

Просто способ организовать работу над программой небольшими этапами. Вместо того чтобы пытаться сделать всё сразу, команда разбивает работу на короткие периоды, проверяет результат и продолжает.

![Project tracking template  Jira](https://images.openai.com/static-rsc-4/83OBou1lKxax9xhXbGMzmYilMILgJxM2oKYyPjSda0_Qoq9oAtN4pWVCKAXzzqamA_QlHvlzijJRWAlAz3lN7RIVAOk99epkEcozd2yxKhDHAVZ1waq2f6151RR3bkWO7iT-Ag-50IYPTG7CMdVMNA9ai4_oMr-jsqOrt0RwPOOdz3PA4GIrN8Ho5jhz1XSO?purpose=fullsize)

Jira

Обычная программа для учёта задач. Можно создать список дел, назначить исполнителей и перемещать карточки между колонками «Нужно сделать», «В работе» и «Готово».

![A man's hand holds a pen and writes a check list with checkboxes, a wooden table Time management concept](https://images.openai.com/static-rsc-4/S67JExX21Vo-svwEuz7wsFWUhtb18jB7M2I8n_VxX0FIaVR_NuftHWelhWmojC5Tvjxjw61hqDbnowp9-8LktBEAhw3a94saeEnBKx-47ATUS0utV9mRhFvR0eyK8kOyFpCJVHNjucvVyzhutr_5aCxmCMuEDi35mXHrkviUwRGUFxkmxLOob1AMw3W1ktGV?purpose=fullsize)

Backlog

Список всего, что когда-либо потребуется сделать в проекте. Например: создать страницу входа, сделать регистрацию, добавить меню, исправить ошибки.

![Calendar Weekly plan Doing business or activities with in a week](https://images.openai.com/static-rsc-4/YQgNL4Gm3vDYkxtQA9U0cy4H1lXx22Rev8fp3vxcWljIRx29Vj_tdcMkG5ZfBkDEWhAHpzij-IcaTGaUvbAfG8sB9pAIJZnFSkiveRYbL6o_FHs_gtdobXQnSbure6WkTqQ1VtqFcJf2DxPGlkPCNchnCDEbF_e43pc_1NC3UeHDH1DcpqXwXxLeZCmlg-9F?purpose=fullsize)

Sprint

Определённый промежуток времени, обычно одна или две недели, за который команда планирует выполнить часть задач. Это просто рабочий цикл с установленными началом и концом.

![UX graphic designer planning application process development prototype wireframe for web smart phone](https://images.openai.com/static-rsc-4/K02vnlQz_UdVnlCjHkcd_-RBHuAR73i97WOnRnarua8Po9jy2WN6W1zgbmUvnj5gHiXSj1Ss9bF9xujBq9WR77OV3_wguPlUlB2EID0IKFNKwNyxgL54IQ1mmgnGhjGPIoxDDspmOzMMtlkI5ElX03bMMmSWdQOBnphFePKvf-6DNfQX2e892FDcPgXG7URe?purpose=fullsize)

User Story

Описание того, что пользователь хочет получить от программы. Например: «Как пользователь, я хочу создать аккаунт, чтобы просматривать свои предыдущие покупки».

![Murata Is Looking for Partners to Create the Future Murata Open Innovation｜Murata Manufacturing](https://images.openai.com/static-rsc-4/xpHl6GtaKTJv4zDNV2PxvcjP2c19kp1C7qpGSRKEH4-la9xdn7xr1epl-RV2ZPyVVVHf-VImT8CFW8xDufKdQpsq8ynJeuOjubIbB2G2RbykA7WIe8CoN_t0g-NnAa2xnCO3T8h8OQWGknR6B2PCrehREQztXnUYNgQ-nXelBVKmV4rMhBSHU52RF-3cPmuD?purpose=fullsize)

Daily Standup

Короткое ежедневное собрание, на котором каждый говорит, что сделал вчера, что собирается делать сегодня и что ему мешает.

![Blog sobre project management y trabajo en equipo con Projoodle](https://images.openai.com/static-rsc-4/yaP8wmOflbr1A3NKPE5OdpAyvzh1dAQ8qkWubI2y6TxDPBrpG6-9kA5JJmRR4bijzY2XhxzUQ4GyegYtbhVam-4Wb8YGatlHjRJL3Hd6bpeffwINiIakVgmux18Mbp9cptPbB6erxpoCSnECseaVeldYmLRqi5KYA9RdwL4Lz1xDF_zeMAvcjA3EXbJpMhhT?purpose=fullsize)

Sprint Review

Демонстрация того, что команда успела сделать за рабочий цикл. По сути, показать работающий результат и получить отзывы.

![婚活成功のための自己分析ワーク婚活カウンセラーが教える実践法｜たけさん@婚活カウンセラー](https://images.openai.com/static-rsc-4/yvMkftnnYWOdWZIXeZ6ZHInM4_zUodmjO6CoucdhZQCpkg2dH_kvlhFQuNFGSmDiT3C78e2oAyMLzfD9_F2VNeKsUd8V0DQQptS6H_1KjzcE9DSCcbNqs6qi3PsiNX6XMaoohHPndovOuEWNPgvgbL8o9s_URKfTCl2XUbT0ghOrWyWkmN_hMjcn0_EiXcq_?purpose=fullsize)

Retrospective

Обсуждение после завершения цикла: что получилось, что не получилось и что можно изменить в следующий раз.

    </main>
</body>
</html>

