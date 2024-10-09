# Atividade em Grupo - Sistema de uma Biblioteca
Atividade em Grupo de Lógica de Programação


        Var
        genero:inteiro
        acao:inteiro
        estado:inteiro
        disponibilidade:inteiro
        multa:real
        atraso:real
        diasEmprestimo:inteiro
        categoria:caractere
        livro:inteiro
        livroRenova:caractere
        diasRenova:inteiro
        totalRenova:inteiro
        nome, senha: caractere
        cadas_telefone: inteiro
        telefone: inteiro
        verificacao: inteiro
        
        
        Inicio
        // Seção de Comandos, procedimento, funções, operadores, etc...
        
        totalRenova <- 0
        
        escreval("Bem-vindo à biblioteca")
        escreval("Login")
        escreval("Nome: ")
        leia(nome)
        escreval("Senha: ")
        leia(senha)
        
        escreval("Você já cadastrou o seu numero de telefone? ")
        escreval("[1] - Sim")
        escreval("[2] - Não")
        leia(cadas_telefone)
        
        escolha cadas_telefone
                caso 2
                     escreval("Digite o seu numero de telefone: ")
                     leia(telefone)
                     escreval("Verificação de telefone ")
                     escreval("O seu numero de telefone é: ", telefone, " ? ")
                     escreval("[1] - Sim ")
                     escreval("[2] - Não ")
                     leia(verificacao)
                     escolha verificacao
                             caso 2
                                  repita
                                     escreval("Digite o seu numero de telefone: ")
                                     leia(telefone)
                                       escreval("Verificação de telefone ")
                                       escreval("O seu numero de telefone é: ", telefone, " ? ")
                                       escreval("[1] - Sim ")
                                       escreval("[2] - Não ")
                                       leia(verificacao)
                                  ate verificacao = 1
                     fimescolha
        fimescolha
        
        repita
        
             escreval("O que você deseja fazer?")
             escreval("   [1] Empréstimo")
             escreval("   [2] Devolução")
             escreval("   [3] Reempréstimo")
             escreval("   [4] Sair")
             leia(acao)
        
             escolha acao
        
                     caso 1
        
                          escreval("Qual o gênero do livro selecionado?")
                          escreval("   [1] Ficção")
                          escreval("   [2] Suspense")
                          escreval("   [3] Estudos")
                          escreval("   [4] Mistério")
                          escreval("   [5] Romance")
                          escreval("   [6] Clássicos")
                          leia(genero)
        
                     escolha genero
        
                             caso 1
        
                                   escreval("Você selecionou a categoria Ficção")
                                   escreval("Qual livro você prefere ler? ")
                                   escreval("   [1] - Duna")
                                   escreval("   [2] - Admirável mundo novo")
                                   leia(livro)
                                   escolha livro
                                          caso 1
                                               escreval("Você selecionou o livro Duna " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
        
                                          caso 2
                                               escreval("Você selecionou o livro Admirável Mundo Novo " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
        
                                   fimescolha
        
        
        
        
                             caso 2
        
                                       escreval("Você selecionou a categoria Suspense")
                                       escreval("Qual livro você prefere ler? ")
                                       escreval("   [1] - Olhos vazios")
                                       escreval("   [2] - A Paciente Silenciosa")
                                       leia(livro)
                                       escolha livro
                                          caso 1
                                               escreval("Você selecionou o livro Olhos vazios " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
        
                                          caso 2
                                               escreval("Você selecionou o livro A paciente silenciosa " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
        
                                      fimescolha
                            caso 3
        
                                  escreval("Você selecionou a categoria Estudos")
                                  escreval("Qual livro você prefere ler? ")
                                       escreval("   [1] - O Algebrista ")
                                       escreval("   [2] - Como se faz uma tese")
                                       leia(livro)
                                       escolha livro
                                          caso 1
                                               escreval("Você selecionou o livro O Algebrista " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
        
                                          caso 2
                                               escreval("Você selecionou o livro Como Se Faz Uma Tese " )
                                               escreval("Por quanto tempo você deseja emprestar o livro?")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
        
                                      fimescolha
                            caso 4
        
                                  escreval("Você selecionou a categoria Mistério")
                                  escreval("Qual livro você prefere ler? ")
                                       escreval("   [1] - O Assassinato No Expresso do Oriente ")
                                       escreval("   [2] - Morte No Nilo")
                                       leia(livro)
                                       escolha livro
                                          caso 1
                                               escreval("Você selecionou o livro O Assassinato No Expresso do Oriente " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
                                          caso 2
                                               escreval("Você selecionou o livro Morte No Nilo " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
                                       fimescolha
        
                            caso 5
        
                                  escreval("Você selecionou a categoria Romance")
                                  escreval("Qual livro você prefere ler? ")
                                       escreval("   [1] - Orgulho E Preconceito ")
                                       escreval("   [2] - A Culpa É Das Estrelas ")
                                       leia(livro)
                                       escolha livro
                                          caso 1
                                               escreval("Você selecionou o livro Orgulho E Preconceito " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
                                          caso 2
                                               escreval("Você selecionou o livro A Culpa É Das Estrelas " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
                                       fimescolha
        
                            caso 6
        
                                  escreval("Você selecionou a categoria Clássicos")
                                  escreval("Qual livro você prefere ler? ")
                                       escreval("   [1] - Romeu E Julieta ")
                                       escreval("   [2] - Robin Hood")
                                       leia(livro)
                                       escolha livro
                                          caso 1
                                               escreval("Você selecionou o livro Romeu E Julieta " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
                                          caso 2
                                               escreval("Você selecionou o Robin Hood " )
                                               escreval("Por quanto tempo você deseja emprestar o livro")
                                               leia (diasEmprestimo)
                                               se (diasEmprestimo > 30) entao
                                                  diasEmprestimo <- 30
                                                  escreval("Você deve entregar o livro em 30 dias, pois esse é o tempo limite da biblioteca. O tempo de empréstimo já foi atualizado")
                                                  senao
                                                       escreval("Você vai emprestar o livro durante ", diasEmprestimo, " dias")
        
                                               fimse
                                       fimescolha
        
        
                     fimescolha
        
                     caso 2
                          escreval("Qual o estado do livro?")
                          escreval("   [1] Em dia")
                          escreval("   [2] Em atraso")
                          leia(estado)
        
                          se estado = 2 entao
                             escreval("Quantos dias o livro está em atraso?")
                             leia(atraso)
        
                             multa <- atraso*1.5
                             escreval("Você deve pagar", multa, " reais de multa pelo atraso")
        
                          senao
                               escreval("Escreva o gênero do livro selecionado")
                               escreval("    Ficção")
                               escreval("    Suspense")
                               escreval("    Estudos")
                               escreval("    Mistério")
                               escreval("    Romance")
                               escreval("    Clássicos")
                               leia(categoria)
                               escreval("Você devolveu o livro do gênero ", categoria)
        
                          fimse
        
                     caso 3
                          escreval("Escreva o título do livro que você quer renovar")
                          leia(livroRenova)
                          
                          escreval("Por quanto tempo você deseja renovar o livro?")
                          leia(diasRenova)
                          
                          se (diasRenova > 15) entao
                             escreval("Valor inválido, o total de dias para a renovação foi alterado para 15 dias")
                             diasRenova <- 15
                             fimse
                          totalRenova <- totalRenova + 1
                          
                          se (totalRenova = 5) entao
                             escreval("Digite outra ação, o livro já foi renovado 5 vezes, é necessário devolvê-lo")
                             senao
                             
                                  escreval("Livro renovado por: ", diasRenova, " dias. Lembre-se que você pode renovar o livro mais ", 5-totalRenova, " vezes.")
                                  fimse
                          
        
             fimescolha
        ate (acao = 4)
        
        
        Fimalgoritmo
