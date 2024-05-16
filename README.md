# TCC-GSC-2024.1
# Exemplo de código utilizado no artigo de TCC.

# Importar bibliotecas necessárias
import time

# Definir funções para simular ações do robô
def mover_braco_esquerdo(posicao):
  print(f"Movendo braço esquerdo para posição {posicao}")
  time.sleep(1)

def mover_braco_direito(posicao):
  print(f"Movendo braço direito para posição {posicao}")
  time.sleep(1)

def usar_instrumento(instrumento, acao):
  print(f"Usando {instrumento} para {acao}")
  time.sleep(1)

# Simular a preparação para a cirurgia
print("Preparando o robô da Vinci XI para a cirurgia...")
mover_braco_esquerdo("posição inicial")
mover_braco_direito("posição inicial")
usar_instrumento("tesoura cirúrgica", "esterilizar")

# Simular a incisão
print("Iniciando a incisão...")
mover_braco_direito("posição de incisão")
usar_instrumento("bisturi", "incisar")

# Simular a dissecção
print("Dissecando o tecido...")
mover_braco_esquerdo("posição de dissecção")
usar_instrumento("pinça", "segurar tecido")
mover_braco_direito("movimentos de dissecção")

# Simular a sutura
print("Sutura da incisão...")
mover_braco_direito("posição de sutura")
usar_instrumento("agulha de sutura", "sutura")

# Simular a finalização da cirurgia
print("Finalizando a cirurgia...")
mover_braco_esquerdo("posição inicial")
mover_braco_direito("posição inicial")
print("Cirurgia concluída com sucesso!")
