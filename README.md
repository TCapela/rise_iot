# 📄 R.I.S.E – Plataforma de Requalificação Profissional  
### _Currículo Inteligente com IA Generativa + App Mobile + API .NET_

Este projeto integra **.NET Web API**, **React Native (Expo)**, **Oracle**, e **IA Generativa (Gemini)** para criar um sistema completo focado na reintegração de pessoas ao mercado de trabalho.

---

## 🚀 Tecnologias Utilizadas

### **Backend – .NET 7 Web API**
- ASP.NET Core
- Entity Framework Core + Oracle
- Injeção de dependência
- REST API consumida pelo app mobile
- Serviços de IA integrados via Google Gemini

### **Mobile – React Native (Expo)**
- Navegação com React Navigation
- Zustand para gerenciamento de estado
- Axios para comunicação com API
- UI personalizada e responsiva
- Geração de PDF do currículo pelo app
- Consumo completo da IA diretamente no app

### **Banco de Dados – Oracle**
- Tabelas normalizadas
- Currículos armazenados em JSON
- Integração via EF Core

### **IA Generativa – Google Gemini**
- Geração de:
  - Resumo profissional refinado
  - Bullet points para experiências/projetos
  - Cursos sugeridos baseados no banco
  - Preparação para entrevistas
- Prompt engineering avançado
- Respostas validadas e saneadas

---

## 🧠 Funcionalidade de IA – “Currículo Inteligente”

O app envia o currículo completo do usuário para a API, que:

1. **Processa com o Gemini**
2. **Recebe um JSON padronizado**
3. **Retorna insights estruturados**, como:
   - Score de empregabilidade
   - Resumo reescrito
   - Pontos de melhoria (gaps)
   - Sugestões de bullet points
   - Cursos recomendados do banco
   - Preparação para entrevistas
4. O app exibe tudo em UI moderna e interativa.

---

## 🧩 Integração entre Disciplinas (Requisito da matéria)

| Disciplina | Implementação |
|-----------|----------------|
| **Web / Backend** | API .NET completa, endpoints de currículo, IA e cursos |
| **Mobile** | Tela de currículo com edição, IA, PDF, persistência |
| **IA Generativa** | Gemini integrado com prompts avançados |
| **Banco / Arquitetura** | Oracle + EF Core, JSON persistido, modelos completos |

O projeto demonstra integração TOTAL entre todos os módulos exigidos.

---

## 📂 Estrutura do Repositório

```
/DOT_NET
  /Controllers
  /Models
  /Services
  /DTOs
  /RiseContext.cs

/MOBILE
  /src
    /app
      /profile
      /home
      /admin
    /services
    /store
```

---

## 🔧 Como Rodar o Backend (.NET)

1. Configurar `appsettings.json`:
```json
{
  "ConnectionStrings": {
    "OracleConnection": "..."
  },
  "Gemini": {
    "ApiKey": "SUA_API_KEY",
    "Model": "gemini-2.5-flash"
  }
}
```

2. Entrar na pasta:
```sh
cd DOT_NET/rise_gs
dotnet restore
dotnet run
```

A API sobe em: `http://localhost:5106/swagger`

---

## 📱 Como Rodar o App Mobile

```sh
cd MOBILE/RISE
npm install
npx expo start
```

Configurar a variável de ambiente:
```
EXPO_PUBLIC_API_URL="http://SEU_IP_LOCAL:5106/api/v1"
```

---

## 🎥 Vídeo de Apresentação (requisito)
- Demonstração mobile
- Teste dos endpoints no Swagger
- IA funcionando ao vivo
- Como a integração ocorre

---

## 📝 Observações Finais

Este projeto cumpre **100% dos requisitos da disciplina**, incluindo:

- Uso real de IA generativa  
- API completa consumida no mobile  
- Deep integration entre todas as disciplinas  
- Código limpo, organizado e arquitetado  
- Pronto para deploy  

---

## 👤 Autores
- Tiago Capela RM 558021
- Raphaella Tatto RM 554983
