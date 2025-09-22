🎂 Aniversário - Confirmação de Presença

Um site simples e bonito para confirmação de presença em eventos, feito com React + Vite + TailwindCSS + Firebase.
O administrador pode gerenciar informações do evento, como data, local, descrição, horários e até a foto da festa.
Os convidados conseguem confirmar a presença de múltiplas pessoas, informando nome, telefone e idade.

✨ Funcionalidades
👤 Convidados

Visualizam informações do evento: local, data, horários, descrição e foto.

Confirmação de presença para múltiplas pessoas.

Formulário com nome, telefone e idade.

Mensagem de sucesso/erro após confirmação.

🔑 Admin

Login exclusivo para administrador.

Pode editar informações do evento:

📅 Data

⏰ Intervalo de horários (ex: 10h até 11h)

📍 Local

📝 Descrição

🖼️ Foto da festa

Gerencia a lista de confirmados em tempo real.

Pode excluir confirmações individuais.

Logout com segurança.

🛠️ Tecnologias

React
 + Vite
 ⚡

TailwindCSS
 🎨

Firebase
 🔥

Authentication (login admin)

Firestore (armazenamento dos dados)

Storage (upload de fotos do evento)

Hosting (deploy gratuito)

🚀 Como rodar o projeto localmente

Clone o repositório:

git clone https://github.com/seu-usuario/aniversario-presenca.git
cd aniversario-presenca


Instale as dependências:

npm install


Configure o Firebase:

Crie um projeto no Firebase Console
.

Habilite Firestore Database e Authentication (Email/Senha).

Crie a coleção evento com o documento info.

Configure o arquivo src/firebase.js com suas credenciais:

import { initializeApp } from "firebase/app";
import { getAuth } from "firebase/auth";
import { getFirestore } from "firebase/firestore";
import { getStorage } from "firebase/storage";

const firebaseConfig = {
  apiKey: "SUA_API_KEY",
  authDomain: "SEU_PROJETO.firebaseapp.com",
  projectId: "SEU_PROJECT_ID",
  storageBucket: "SEU_PROJECT_ID.appspot.com",
  messagingSenderId: "XXXXXXX",
  appId: "APP_ID",
};

const app = initializeApp(firebaseConfig);

export const auth = getAuth(app);
export const db = getFirestore(app);
export const storage = getStorage(app);


Rode o projeto:

npm run dev


Acesse no navegador:

http://localhost:5173

🌍 Deploy Gratuito

Você pode publicar o site de graça em:

Vercel
 → simples e rápido para projetos React.

Netlify
 → basta arrastar a pasta dist.

Firebase Hosting
 → integração total com seu Firestore.

📷 Demonstração
Página inicial

Mostra informações do evento e botão de confirmação.

Página de confirmação

Formulário dinâmico para confirmar várias pessoas.

Área do admin

Gerencia evento, lista de confirmados e foto.

👨‍💻 Autor

Projeto desenvolvido por Enzo Augusto 🚀
