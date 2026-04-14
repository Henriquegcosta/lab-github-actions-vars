# Respostas para a reflexão:

1. Por que a Secret aparece como ***? 

   O GitHub mascara automaticamente qualquer valor vindo do contexto de secrets nos logs para evitar vazamento de dados sensíveis (senhas, chaves de API).
          
3. O Job 2 consegue ler a BUILD_VERSION do Job 1? 

   Não. Variáveis de Job são isoladas. Para passar dados entre Jobs, precisaríamos usar 'outputs' ou artefatos.
