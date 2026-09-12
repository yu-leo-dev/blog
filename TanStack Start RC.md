# Изучаем TanStack Start

## 1. [Getting Started](https://tanstack.com/start/latest/docs/framework/react/getting-started)

```bash
bunx @tanstack/cli create my-tanstack-app
```

Выбираем React, Biome, Nitro, demo/examples - No.
В add-ons пока ничего не выбираем (позже попробовать Strapi, Compiler, Drizzle, Shadcn, T3Env, Apollo Client, Tanstack Query).
Git - No.

⚠️ Agent skills: yes; TanStack Intent configured

⚠️ Command "bunx --bun @tanstack/intent install" did not run successfully. Please run this manually in your project.

Как все это отключить? Ответ: --no-intent

```bash
cd my-tanstack-app
bun dev
```

Ok. Запускается. Работает.

ℹ️ Чтобы не было ошибок гидрации в консоли Chrome, желательно максимально отключить расширения в Chrome.

```bash
bun run build
bun preview
```

⚙️ Размер основного JS-бандла: 314 kB (всего 5 запросов, 322 kB)

⚠️ Почему-то нет файла favicon.ico (в прошлых версиях, вроде, был).

⚠️ Nitro 3 все еще в стадии beta.

### Попробуем абсолютно минимальный проект

```bash
bunx @tanstack/cli create my-tanstack-app --blank --no-git --yes
```
Все то же самое, только нет Nitro (билдится не в папку ./output, а в ./dist). Нет Tailwind и DevTools.

⚙️ Размер основного JS-бандла: 314 kB (всего 5 запросов, 317 kB)

## Examples

Можно выбрать примеры.

**Events** - появились коллекции и документы, а также AI assistant. Интересно. Позже изучить

```
Starting content-collections with config content-collections.ts
... finished build of 2 collections and 14 documents in 491ms
```

Добавились: @tanstack/ai-...

⚙️❗ Размер основного JS-бандла: 498 kB (всего 33 запроса, 4.1 MB)

**Resume**

Добавились: shadcn UI, @tanstack/ai-...
⚙️❗ Размер основного JS-бандла: 989 kB (всего 6 запросов, 2.1 MB)

### Моя итоговая конфигурация

```bash
bunx @tanstack/cli create my-tanstack-app --yes --toolchain biome --deployment nitro --no-intent

```
⚙️ Размер основного JS-бандла: 321.01 kB (Добавилось demo. Всего 8 запросов, 473 kB. Из них 2 шрифта Fraunces суммарно около 100 kB). Demo - в принципе, нормально. Готовый Layout, переключатель dark/light.
