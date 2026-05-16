# MapFood Web (Frontend)

Aplicação front-end moderna para a plataforma MapFood, focada em conectar consumidores a produtores locais e eventos.

## 🚀 Tecnologias

- **React 18**
- **Vite**
- **TypeScript**
- **Tailwind CSS**
- **Shadcn/UI** (Radix UI)
- **React Query** (TanStack Query)
- **React Hook Form** + **Zod**

## 🏗️ Arquitetura

O projeto é organizado de forma modular:
- `components/ui`: Componentes de interface baseados no Radix UI.
- `pages`: Componentes de página que representam as rotas da aplicação.
- `services`: Camada de integração com a API.
- `hooks`: Hooks customizados para lógica reutilizável.
- `lib`: Utilitários e configurações (ex: máscaras, classes tailwind).

## ⚙️ Instalação e Uso

1.  Instale as dependências:
    ```bash
    npm install
    ```
2.  Inicie o servidor de desenvolvimento:
    ```bash
    npm run dev
    ```

## ⚠️ Pontos de Atenção

- **Segurança no Login:** Atualmente o login é simulado buscando todos os usuários da API e filtrando localmente. **Isso é uma falha crítica de segurança** e deve ser corrigido com a implementação de autenticação JWT no backend.
- **Configuração da API:** A URL da API está fixada no arquivo `src/services/api.ts`. Recomenda-se utilizar variáveis de ambiente (`.env`).
