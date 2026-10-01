# 📝 Anotações & Registro de Aprendizado: Semana 01

> **Tema:** Fundamentos de SQL, Banco de Dados & Power Query  
> **Período:** Dias 01 a 07  
> **Status:** [ ] Não iniciado | [ ] Em andamento | [ ] Concluído

---

## 🎯 Metas da Semana
- [ ] Dominar a sintaxe básica e intermediária de SQL (`SELECT`, `WHERE`, `GROUP BY`, `HAVING`).
- [ ] Praticar todos os tipos de `JOIN` e entender quando usar subconsultas.
- [ ] Executar transformações e limpezas com Power Query (Pivot/Unpivot, Merge e Append).

---

## 📌 Principais Conceitos Aprendidos

### 1. SQL & Bancos Relacionais
* **Resumo:** *(Insira aqui anotações sobre PK/FK, modelagem relacional, etc.)*
* **Comandos / Sintaxe-Chave:**
```sql
-- Exemplo de consulta com agregação e filtro agrupado
SELECT 
    categoria_id,
    COUNT(produto_id) AS total_produtos,
    AVG(preco) AS media_preco
FROM produtos
WHERE status = 'ATIVO'
GROUP BY categoria_id
HAVING AVG(preco) > 50.00
ORDER BY media_preco DESC;
```

### 2. Joins & Relacionamentos
* **Diferença prática observada:**
  - `INNER JOIN`: Apenas registros correspondentes em ambas as tabelas.
  - `LEFT JOIN`: Todos da tabela à esquerda + correspondentes da direita (preenche nulos onde não houver match).

### 3. Power Query & ETL
* **Etapas importantes aplicadas:**
  - Tratamento de nulos / Tipagem de colunas.
  - Uso do *Unpivot* para transformar colunas em formato tabular adequado para modelagem.

---

## 🧪 Exercícios & Projetos Práticos Realizados
| Data | Tópico / Exercício | Plataforma / Origem | Link / Arquivo |
| :--- | :--- | :--- | :--- |
| Dia 02 | Exercícios de Agregação | SQLBolt / HackerRank | [Link ou anotação] |
| Dia 04 | Desafios de Joins | LeetCode / Banco Local | [Link ou anotação] |
| Dia 07 | Tratamento de Vendas | Power Query | `projeto-vendas.pbix` |

---

## ❓ Dúvidas & Pontos de Atenção para Revisar
- [ ] *Exemplo: Revisar a diferença prática de performance entre CTEs e Subqueries.*
- [ ] 

---

## 🏆 Autoavaliação da Semana
- **O que foi mais fácil?** 
- **O que exigiu mais tempo/esforço?** 
- **Pronto para avançar para a Semana 2?** ( ) Sim  ( ) Preciso revisar mais 1 dia
