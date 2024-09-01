# Podcast Manager

## Description

Podcast Manager is an application inspired by the Netflix style, which allows you to centralize different podcast episodes separated by category. This project aims to facilitate access and organization of podcast episodes in video format, providing an intuitive and pleasant navigation experience for users.

## Features

- **List podcast episodes in category sessions:** Episodes are organized into categories such as health, bodybuilder, mindset and humor, allowing users to easily explore the available content.
- **Filter episodes by podcast name:** Users can perform specific searches by podcast name, making it easier to access the desired episodes.

## Implementation

### List podcast episodes in category sections

- **Endpoint:** `GET /list`
- **Description:** Returns a list of podcast episodes organized by categories.
- **Example answer:**

```json
[
  {
    "podcastName": "flow",
    "episode": "CBUM - Flow #319",
    "videoId": "pQSuQmUfS30",
    "cover": "https://i.ytimg.com/vi/pQSuQmUfS30/maxresdefault.jpg",
    "link": "https://www.youtube.com/watch?v=pQSuQmUfS30",
    "categories": ["saúde", "esporte", "bodybuilder"]
  },
  {
    "podcastName": "flow",
    "episode": "RUBENS BARRICHELLO - Flow #339",
    "videoId": "4KDGTdiOV4I",
    "cover": "https://i.ytimg.com/vi/4KDGTdiOV4I/maxresdefault.jpg",
    "link": "https://www.youtube.com/watch?v=4KDGTdiOV4I",
    "categories": ["esporte", "corrida"]
  }
]
```

### Filter episodes by podcast name

- **Endpoint:** `GET /episode?podcastName={nome}`
- **Description:** Returns a list of podcast episodes based on the given podcast name.
- **Request example:**`GET /episode?podcastName=flow`

## Technologies Used

- **[TypeScript](https://www.typescriptlang.org/):** Linguagem de programação utilizada para o desenvolvimento do projeto.
- **[Tsup](https://github.com/egoist/tsup):** Ferramenta de construção e empacotamento para projetos TypeScript.
- **[Tsx](https://github.com/egoist/tsx):** Compilador TypeScript que suporta a construção de projetos.
- **[Node.js](https://nodejs.org/):** Ambiente de execução JavaScript que permite executar código JavaScript do lado do servidor.
- **[@types/node](https://www.npmjs.com/package/@types/node):** Pacote de definições de tipos para Node.js para auxiliar no desenvolvimento com TypeScript.

## How to Use

1. Clone this repository.
2. Install dependencies using `npm install`.
3. Start the server by running `start:dev`.
4. Access the provided endpoints to list podcast episodes or filter them by podcast name.

## Contribution

Contributions are welcome! Feel free to open issues or send pull requests to improve this project.

## License

This project is licensed under the [MIT License](LICENSE).
