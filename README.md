# O Amor é um Commit para a Vida Inteira

class Relacionamento:
    def __init__(self, Gustavo, Rutiele):
        self.nome1 = Gustavo
        self.nome2 = Rutiele
        self.commits = []

    def adicionar_commit(self, commit_msg):
        self.commits.append(commit_msg)
        print(f"[{self.nome1} + {self.nome2}] Commit registrado: '{commit_msg}'")

    def pull_request(self):
        print(f"\n{self.nome1} faz um pull request para o coração de {self.nome2}... 💖")
        print(f"{self.nome2} aceita o PR! O merge foi perfeito! 🎉")
        self.adicionar_commit("Merge do amor: commit realizado com sucesso!")

    def git_push(self):
        print(f"\n{self.nome1} faz git push... Enviando amor para o repositório da vida!")
        print(f"{self.nome1} empurra o commit com a mensagem: 'Te amo!'")
        print(f"{self.nome2} aceita o commit: 'Aceito com todo o meu coração!'")
        print("Amor consolidado no repositório compartilhado. 💑")

    def listar_commits(self):
        print("\nHistórico de commits do nosso relacionamento:")
        for i, commit in enumerate(self.commits, 1):
            print(f"{i}. {commit}")

# Simulação de um relacionamento Git-based
relacionamento = Relacionamento("Gustavo", "Rutiele")

# Gustavo faz um commit
relacionamento.adicionar_commit("Primeiro commit: Declarando meu amor por Rutiele!")

# Gustavo faz pull request
relacionamento.pull_request()

# Rutiele faz git push de volta para o repositório
relacionamento.git_push()

# Listar os commits do relacionamento
relacionamento.listar_commits()
