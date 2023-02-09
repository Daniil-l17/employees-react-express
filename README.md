# Создаем новое Express приложение
## Установим express-generator
```
npm install -g express-generator
```

## Сгенерируем новое express приложение без view(без папки с html файлами)
```
express --no-view
```

## Установка Prisma

Установим Prisma CLI в dev зависимости

```
npm install prisma --save-dev
```

Инициализируем папку Prisma в приложении и указываем SQLite как базу данных
```
npx prisma init --datasource-provider sqlite
```

Создать нужные модели в папке
```
prisma/schema.prisma
```

Делаем миграцию созданных моделей в нашу базу данных
```
npx prisma migrate dev --name init
```