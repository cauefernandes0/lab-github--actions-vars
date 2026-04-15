## CTT

# 1. Por que o secret aparece como ***?
   Porque o GitHub mascara automaticamente secrets nos logs por segurança.

# 2. deploy_app consegue ler BUILD_VERSION?
  Não,pois cada job roda em máquinas diferentes, variáveis não são compartilhadas automaticamente entre elas. Apenas funcionaria se você usasse: artifacts, outputs ou cache
