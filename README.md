Aqui está o texto pronto para você copiar e colar, com os títulos em destaque:

# Controle de Servomotor por PWM com Raspberry Pi Pico W

## Descrição do Projeto
Este projeto demonstra o controle integrado de um servomotor utilizando o microcontrolador **Raspberry Pi Pico W**. Foram implementadas as seguintes funcionalidades:

- **Controle de Servomotor via PWM:** O controle do ângulo é realizado através de **PWM (Pulse Width Modulation)**, simulando o comportamento de um servomotor padrão.  
- **Movimentação Suave:** Implementação de uma rotina para movimentação suave do servo entre 0 e 180 graus.  
- **Experimento com LED RGB:** Testes utilizando a ferramenta educacional **BitDogLab** para observar o comportamento de um LED RGB.

O código foi desenvolvido em **C** com o uso do **Pico SDK** no ambiente **VS Code** e simulado utilizando o **Wokwi**.

## Requisitos do Projeto
1. **Configuração do PWM**  
   - Utilização da GPIO 22 com frequência de aproximadamente **50Hz** (período de 20ms).

2. **Controle do Servomotor**  
   - Ciclo ativo de **2.400µs** para posicionar o servo em **180 graus** (aguardar 5 segundos).  
   - Ciclo ativo de **1.470µs** para posicionar o servo em **90 graus** (aguardar 5 segundos).  
   - Ciclo ativo de **500µs** para posicionar o servo em **0 graus** (aguardar 5 segundos).

3. **Movimentação Suave**  
   - Rotina para movimentação suave do servo entre **0 e 180 graus**, com incrementos de ±5µs e atraso de 10ms.

4. **Experimento com LED RGB (GPIO 12)**  
   - Teste do comportamento do LED RGB utilizando a ferramenta educacional **BitDogLab**.

## Componentes Utilizados
- **Microcontrolador**: Raspberry Pi Pico W  
- **Servomotor**: Micro servo padrão (simulado no Wokwi)  
- **LED RGB**: Conectado à GPIO 12  
- **Ferramenta Educacional**: BitDogLab

## Configuração do Ambiente
1. Instale o **Pico SDK** conforme a documentação oficial.  
2. Configure o **VS Code** com extensões para desenvolvimento com o **Raspberry Pi Pico W**.  
3. Integre o simulador **Wokwi** ao VS Code.  
4. Clone o repositório ou descompacte os arquivos fornecidos.

## Compilando e Executando o Projeto
1. Abra o VS Code e carregue o projeto.  
2. Compile o código utilizando o **Pico SDK**.  
3. Execute a simulação no **Wokwi**.  
4. Verifique a movimentação do servomotor e o comportamento do LED RGB.

## Resultados e Observações
- O servomotor movimenta-se conforme os parâmetros definidos, atingindo as posições de 0, 90 e 180 graus com estabilidade.  
- A movimentação suave entre os extremos ocorre de forma fluida, conforme esperado.  
- O LED RGB apresentou comportamentos distintos durante o experimento com a ferramenta **BitDogLab**.

## Demonstração do Projeto
Assista ao vídeo de demonstração onde explico o funcionamento completo do projeto e mostro a placa em ação:

[![Demonstração do Projeto](https://img.youtube.com/vi/2j5G8T745qY/0.jpg)](https://youtu.be/2j5G8T745qY)

## Conclusão
Este projeto integra conceitos fundamentais como o controle de hardware via **PWM**, o uso de ferramentas educacionais para testes práticos, e a manipulação de LEDs e servomotores. É uma excelente oportunidade para consolidar o conhecimento em sistemas embarcados com o **RP2040**.

## Autor
**Eduardo Medeiros Magalhães**

---

Este projeto foi desenvolvido como parte da Tarefa Individual da Unidade 4 | Capítulo 7 do curso ministrado pelo Prof. Dr. Ricardo Menezes Prates.

> Para mais informações, consulte o enunciado oficial da tarefa ou entre em contato com o autor.
