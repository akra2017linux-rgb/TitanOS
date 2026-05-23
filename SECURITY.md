# Política de Segurança

## Relatar uma Vulnerabilidade de Segurança

Na TitanOS, a segurança é uma prioridade máxima. Se você descobrir uma vulnerabilidade de segurança, por favor, **não abra uma issue pública**. Em vez disso, reporte responsavelmente ao nosso time de segurança.

### Como Reportar

**Email**: security@titanos.io

Por favor inclua o máximo de informações possível:

- Descrição detalhada da vulnerabilidade
- Passos para reproduzir
- Potencial impacto
- Sugestões de fix (se houver)

### O que Esperar

1. **Reconhecimento**: Enviaremos um email confirmando o recebimento dentro de 48 horas
2. **Avaliação**: Nós avaliaremos a severidade dentro de 5-7 dias úteis
3. **Coordenação**: Trabalharemos com você para entender e resolver a vulnerabilidade
4. **Fix**: Quando um fix está pronto, você será notificado antes da publicação
5. **Crédito**: Você receberá crédito público (a menos que prefira permanecer anônimo)

## Cronograma de Disclosure

Nós preferimos coordenar a divulgação de vulnerabilidades:

- **Críticas**: 7 dias para fix e release
- **Altas**: 14 dias para fix e release
- **Médias**: 30 dias para fix e release
- **Baixas**: Até 90 dias para fix e release

## Boas Práticas de Segurança

### Para Usuários

- Mantenha seu TitanOS atualizado
- Use firewall
- Habilite autenticação de dois fatores
- Não desabilite SELinux em produção
- Use senhas fortes
- Monitorar logs do sistema

### Para Desenvolvedores

- Use type hints em Python
- Valide todas as entradas
- Não armazene senhas em plain text
- Use HTTPS para comunicação
- Siga OWASP guidelines
- Faça code review
- Use ferramentas de análise estática