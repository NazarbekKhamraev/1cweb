## BSL kodni tekshirish qoidasi

Har `.bsl` yoki `.os` fayl yaratgach yoki o'zgartirgach:

1. Ishga tushir:
   ```
   java -jar C:/tools/bsl-language-server.jar --analyze --srcDir ./src --reporter json --outputDir ./bsl-report
   ```
2. `./bsl-report` ichidagi JSON hisobotni o'qi.
3. "Error" darajasidagi barcha xatolarni tuza.
4. Toza bo'lgunча 1-3 qadamlarni takrorla.

(Agar MCP ulangan bo'lsa: buyruq o'rniga `analyze_file` tool'ini ishlat.)

## 1C ishlash tartibi

- 1C obyektlari (kengaytma, HTTP-service, rol, metadata) uchun `.claude/skills/` dagi `cc-1c-skills` navyklaridan foydalanish kerak (`/cfe-init`, `/cfe-borrow`, `/meta-compile`, `/role-compile`, `/db-*`, `/web-publish` va h.k.) — qo'lda XML yozish o'rniga.
- Loyiha bazalar/asbob sozlamalari `.v8-project.json` da (sirlarni saqlaydi, git'ga tushmaydi).
- Manba fayllar `src/cfe/<KengaytmaNomi>/` ichida saqlanadi.
