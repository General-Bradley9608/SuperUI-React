<div align="center">

<a href="https://superui.vercel.app/" target="_blank">
  <img src="https://i.ibb.co/CVyrh8b/super-UIBanner8.jpg" width="85%">
</a>

![GitHub releases](https://img.shields.io/github/release/pheralb/superui)
![GitHub stars](https://img.shields.io/github/stars/pheralb/superui)
![GitHub issues](https://img.shields.io/github/issues/pheralb/superui)
![GitHub license](https://img.shields.io/github/license/pheralb/superui)
[![Required Node.JS >= 14.18.0 || >=16.0.0](https://img.shields.io/static/v1?label=node&message=14.18.0%20||%20%3E=16.0.0&logo=node.js&color=3f893e)](https://nodejs.org/about/releases)

</div>

## 💚 [Supabase Launch Week 5](https://supabase.com/launch-week) Hackathon:

- ✅ [Supabase Auth](https://supabase.com/docs/guides/auth) - User authentication.
- ✅ [Supabase Database](https://supabase.com/docs/guides/database) - save the information of each user-created component.


## 💖 Contributors

|               | ✌️ Socials                                                                              |
| ------------- | --------------------------------------------------------------------------------------- |
| Pablo Hdez    | [GitHub](https://github.com/pheralb/superui) - [Twitter](https://twitter.com/pheralb_)  |
| Nacho Aldama  | [GitHub](https://github.com/nachoaldamav) - [Twitter](https://twitter.com/srdrabx) |
| David Huertas | [GitHub](https://github.com/ikurotime) - [Twitter](https://twitter.com/ikurotime)       |
| Juan Rojas    | [GitHub](https://github.com/Davidr2998) - [Twitter](https://twitter.com/tmchein)        |


## 📦 Packages:

- 🚀 [Turborepo](https://turborepo.org/) - The High-performance Build System for JavaScript & TypeScript Codebases.
- ⚡️ [Nextjs](https://nextjs.org/) - The React Framework for Production.
- ⚒️ [React 18](https://es.reactjs.org/) - A JavaScript library for building user interfaces.
- 💙 [Typescript](https://www.typescriptlang.org/) - A superset of JavaScript.
- 💚 [Supabase](https://supabase.com/) - Build in a weekend.
  Scale to millions.
- 💅 [Chakra UI for docs](https://chakra-ui.com/) - Create accessible React apps with speed.
- 💨 [TailwindCSS for library](https://tailwindcss.com/) - Rapidly build modern websites without ever leaving your HTML.
- 💖 [React-Icons](https://react-icons.github.io/react-icons/) - A flexible icon family for everyone.

## 🚀 Getting Started

1. Clone the repository:

```bash
git clone git@github.com:pheralb/superui.git
```

2. Install dependencies:

```bash
cd superui
npm install
```

3. Create a [Supabase database](https://database.new/) with the following query:

```sql
create table components (
  id bigint generated by default as identity primary key,
  user_id uuid references auth.users not null,
  title text check (char_length(title) > 3),
  description text,
  code text,
  inserted_at timestamp with time zone default timezone('utc'::text, now()) not null
);
```

4. Copy Supabase URL & Anon api key from your database and create a _.env_ file in the /app folder with the following content:

```bash
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=
```

5. Run the following command to start the development server:

```bash
npm run dev
```

And ready 🥳, go to [localhost:3001](http://localhost:3001/).

## 🔑 License

- [MIT License](https://github.com/pheralb/superui).
