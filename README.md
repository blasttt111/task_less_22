# Задание №1

## Запустить Flask-приложение, сохраняющее логи в volume на хосте и маппингом портов.
Основные команды:
  - (`docker build -t flask-logs-app .`)
  - (`docker run -d --name flask-logs -p 5000:5000 -v $(pwd)/logs:/logs flask-logs-app`)

  - Dockerfile

  <img width="412" height="263" alt="image" src="https://github.com/user-attachments/assets/53303e53-c9bc-49aa-b77a-58460e9b48c1" />
|
<img width="1335" height="628" alt="image" src="https://github.com/user-attachments/assets/40a3f8a2-6d0f-4c12-9b9c-3f9ac6199a3a" />
|
<img width="1439" height="381" alt="image" src="https://github.com/user-attachments/assets/f087aaa7-7773-4552-a9f5-2c1a8c33fb84" />

# Задание №2
  1. Создал Dockerfile
  <img width="360" height="179" alt="image" src="https://github.com/user-attachments/assets/33ac4273-4d78-4f70-9436-c583821d6712" />

  2. Создал docker-compose.yml
  <img width="476" height="221" alt="image" src="https://github.com/user-attachments/assets/531f3481-f587-41c7-8320-727688df28b5" />

  3. Запуск
  - (`docker compose up -d --build`)

<img width="1178" height="253" alt="image" src="https://github.com/user-attachments/assets/c3ca7265-862a-4947-88fa-c6fb7d3e34b4" />

<img width="1109" height="474" alt="image" src="https://github.com/user-attachments/assets/ea11cb7c-49f8-4f89-b51b-c5d12008216c" />

<img width="1071" height="690" alt="image" src="https://github.com/user-attachments/assets/c47181c4-20ef-4ec3-83ca-d31f367c0b04" />

# Задание #3
  1. Создаем файл .env
  <img width="840" height="245" alt="image" src="https://github.com/user-attachments/assets/284c435a-d8b9-4c99-80f9-763461019f29" />

  2. Создаем Dockerfile и кладем в каталог `api`
<img width="843" height="193" alt="image" src="https://github.com/user-attachments/assets/9c91e28c-c733-42ef-8b28-389c97ecbc46" />

  3. Создаем конфиг для Nginx
  <img width="577" height="449" alt="image" src="https://github.com/user-attachments/assets/143e355b-61ca-4b8d-917f-16f7d43ba769" />

  4. Создаем docker-compose.yml
  <img width="876" height="794" alt="image" src="https://github.com/user-attachments/assets/e36dccbc-63dd-47b6-a0d4-6dc2112a3049" />
  <img width="673" height="456" alt="image" src="https://github.com/user-attachments/assets/a7b8b0a5-baa0-4377-9088-3737ab09b6ac" />

  5. Собираем и запускаем, сразу покурлим и проверим логи.
    - (`docker compose up -d --build`)
    - (`curl localhost:8080/api/health`)
    - (`docker compose logs -f`)
    <img width="1437" height="994" alt="image" src="https://github.com/user-attachments/assets/ef7bf277-525f-4187-9374-2a18b940d67f" />

<img width="1478" height="949" alt="image" src="https://github.com/user-attachments/assets/8b1d0d13-4032-4e43-9c7f-f0d9ad799978" />

<img width="1501" height="955" alt="image" src="https://github.com/user-attachments/assets/0e535395-af15-4963-a3f0-2bec90baf3ea" />
