# 📝 Atividade Avaliativa – Unidade 5  
## ReactJS – CRUD Pessoas (PF e PJ) com Datas

Repositório da solução:  
👉 https://github.com/fabiulabrandao-154/Atividade_Avaliativa_2_Unidade_5

---

## 🎯 Objetivo da Atividade

Implementar a gravação, edição, listagem e exclusão das seguintes datas:

- **Pessoa Física (PF):** data de nascimento  
- **Pessoa Jurídica (PJ):** data de registro  

As informações devem ser gerenciadas pelo CRUD e armazenadas **localmente** via `localStorage`.

---

## ✔️ O que foi desenvolvido

### **Pessoa Física (PF)**
- Adicionado o campo **dataNascimento** no formulário.
- A classe `PF` foi ajustada para incluir esse atributo.
- O DAO `PFDAOLocalV2.mjs` foi configurado para salvar e recuperar essa data.
- Na listagem, quando o filtro está em *PF*, a coluna **Data Nascimento** é exibida corretamente.

### **Pessoa Jurídica (PJ)**
- Adicionado o campo **dataRegistro** no formulário.
- A classe `PJ` foi atualizada com o atributo de data.
- O DAO `PJDAOLocalV2.mjs` salva e recupera o valor no `localStorage`.
- Na listagem, quando o filtro está em *PJ*, aparece a coluna **Data Registro**.

### **Listagem**
- O nome da coluna muda automaticamente:
  - PF → **Data Nascimento**  
  - PJ → **Data Registro**
- A tela carrega e exibe o valor correto de acordo com o tipo.

### **App.jsx**
- Nenhuma lógica adicional foi necessária.  
- Apenas confirmado que o projeto utiliza o conjunto de rotas da versão V2, conforme orientações.

---

## 📂 Arquivos principais modificados

- `src/objetos/pessoas/PF.mjs`  
- `src/objetos/pessoas/PJ.mjs`  
- `src/objetos/dao/PFDAOLocalV2.mjs`  
- `src/objetos/dao/PJDAOLocalV2.mjs`  
- `src/componentes/cadastrapessoa/PessoaFormOOV2.jsx`  
- `src/componentes/listapessoas/ListaPessoasV2.jsx`  

---

## ▶️ Como executar o projeto

```bash
npm install
npm run dev

