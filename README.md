# 🧰 Dev Resources

Faydalı bulduğum repolar, kurslar ve notlar. Çoğu Claude Code ve AI destekli geliştirme üzerine.
Katkıya açık. Eklemek istediğin bir şey varsa PR gönderebilirsin! 🙌

## 📑 İçindekiler

- [🧠 Hafıza, Context ve Token Tasarrufu](#-hafıza-context-ve-token-tasarrufu)
- [🛠️ Skill Koleksiyonları ve Workflow](#️-skill-koleksiyonları-ve-workflow)
- [🎨 Frontend ve Tasarım](#-frontend-ve-tasarım)
- [✍️ Yazı, Pazarlama ve Görsel](#️-yazı-pazarlama-ve-görsel)
- [🤖 Agent'lar ve Orkestrasyon](#-agentlar-ve-orkestrasyon)
- [🔌 Öne Çıkan MCP Sunucuları](#-öne-çıkan-mcp-sunucuları)
- [🚀 Canlıya Çıkmadan Önce Checklist](#-canlıya-çıkmadan-önce-checklist)
- [🌿 Git Öğren ve GitHub Hileleri](#-git-öğren-ve-github-hileleri)
- [📚 Kurslar](#-kurslar)
- [🧪 Denenecekler](#-denenecekler)
- [🏕️ Boş Zamanda Bak](#️-boş-zamanda-bak)

---

## 🧠 Hafıza, Context ve Token Tasarrufu

- **[Claude-Mem](https://github.com/thedotmack/claude-mem)** → Oturumlar arası hafıza. Projelerini ve dosyalarını hatırlıyor, bir daha baştan anlatmıyorsun.
- **[Headroom](https://github.com/headroomlabs-ai/headroom)** → Seninle model arasında duruyor, logları ve araç çıktılarını sıkıştırıyor. Aynı sonuç, çok daha az token.
- **[OmniRoute](https://github.com/cheaper-inference/OmniRoute)** → Tüm AI modellerine tek endpoint'ten erişim. Bir sağlayıcının kotası bitince otomatik olarak diğerine geçiyor, limit yüzünden kodlama yarım kalmıyor. *(Sağlayıcı hesaplarını / API key'lerini kendin getiriyorsun.)*
- **[avenoxbeyin](https://github.com/avenoxai/avenoxbeyin)** → Claude Code / Codex yanında çalışan yerel "ikinci beyin". Notları Obsidian vault'unda Markdown olarak tutuyor, oturumlar arası hafıza sağlıyor.
- **[Graphify](https://github.com/Graphify-Labs/graphify)** → Kod tabanını (dokümanlar, SQL şemaları, config'ler dahil) sorgulanabilir bir bilgi grafiğine çeviriyor. Grep'lemek yerine `/graphify` ile ilişkileri soruyorsun.
- **[MarkItDown](https://github.com/microsoft/markitdown)** → Microsoft'tan. PDF, Office dosyaları, görseller, HTML hatta YouTube linklerini LLM'e beslemeye hazır Markdown'a çeviriyor.

## 🛠️ Skill Koleksiyonları ve Workflow

- **[Anthropic Skills](https://github.com/anthropics/skills)** → Anthropic'in resmi skill koleksiyonu. Skill nasıl yazılır görmek için en iyi referans; docx/pdf/pptx/xlsx skill'leri de burada.
- **[Claude Code Setup](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/claude-code-setup)** → Anthropic'in resmi eklentisi. Kod tabanını tarıyor; projene uygun hook, skill, alt ajan ve MCP öneriyor, gürültüyü temizliyor. Kurulum: `/plugin install claude-code-setup@claude-plugins-official`
- **[skills (Vercel)](https://github.com/vercel-labs/skills)** → `npx skills` CLI'ı. Agent skill'lerini bulmak, kurmak, güncellemek ve silmek için paket yöneticisi gibi.
- **[Superpowers](https://github.com/obra/superpowers)** → Agent'ı disiplinli bir akışa sokuyor: önce tasarımı netleştir, plan yaz, TDD ile geliştir, her adımda review yap.
- **[Matt Pocock Skills](https://github.com/mattpocock/skills)** → Matt Pocock'un kendi kullandığı skill'ler: gereksinimleri sorgulama, TDD, yapılandırılmış debugging, mimari review, spec ve PR yazımı.
- **[Addy Osmani Agent Skills](https://github.com/addyosmani/agent-skills)** → Spec'ten ship'e tüm geliştirme döngüsünü kapsayan 25 skill. Agent'tan senior mühendis disiplininde çıktı almak için.
- **[Andrej Karpathy Skills](https://github.com/multica-ai/andrej-karpathy-skills)** → Karpathy'nin LLM'lerin kodlama hatalarına dair gözlemlerinden çıkarılmış tek bir CLAUDE.md. Kısaca: varsayımları netleştir, basit tut, sadece gereken yeri değiştir.
- **[ECC](https://github.com/affaan-m/ecc)** → Uzman agent'lar, skill'ler, komutlar, hook'lar, hafıza ve güvenlik taramasını bir arada sunan kapsamlı toolkit. Agent'ı önce planlayıp sonra test ederek doğrulamaya zorluyor.
- **[Ponytail](https://github.com/dietrichgebert/ponytail)** → "En iyi kod hiç yazmadığın koddur" felsefesi. Agent'ın sadece gerekli kodu yazmasını sağlıyor; diff review ve repo audit komutları var.
- **[Task Observer](https://github.com/rebelytics/one-skill-to-rule-them-all)** → Nasıl çalıştığını izliyor, düzeltmelerini öğreniyor, skill'lerini kendi kendine geliştiriyor. Sen onaylamadan hiçbir şeyi değiştirmiyor.
- **[i-have-adhd](https://github.com/ayghri/i-have-adhd)** → Agent'ın cevaplarını aksiyona dönük hale getiriyor: önce sıradaki adım, numaralı görevler, gereksiz giriş/kapanış cümleleri yok.
- **[Context Engineering Skills](https://github.com/muratcankoylan/agent-skills-for-context-engineering)** → Context engineering, multi-agent mimari, hafıza, tool tasarımı ve değerlendirme üzerine skill'ler. Production agent sistemleri kuranlar için.
- **[Trail of Bits Skills](https://github.com/trailofbits/skills)** → Güvenlik firması Trail of Bits'ten. Güvenlik araştırması, açık tespiti, kod audit ve reverse engineering için Claude Code plugin marketplace'i.
- **[Supabase Agent Skills](https://github.com/supabase/agent-skills)** → Supabase'in resmi skill'leri. Supabase ve Postgres best practice'lerini agent'a öğretiyor.

## 🎨 Frontend ve Tasarım

- **[Impeccable](https://github.com/pbakaus/impeccable)** → Agent'a ortak bir tasarım dili veriyor (`critique`, `audit`, `polish`, `bolder` gibi komutlar). "AI yapımı gibi duran" jenerik tasarım kalıplarını da yakalıyor.
- **[UI UX Pro Max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)** → Stil, renk paleti, font eşleşmeleri ve UX kurallarından oluşan aranabilir veritabanı. Ürününe göre design system öneriyor.
- **[Modern Web Guidance](https://github.com/GoogleChrome/modern-web-guidance-src)** → Google Chrome ekibinden. Agent'ları eskimiş kalıplardan uzaklaştırıp modern tarayıcı API'lerine ve güncel best practice'lere yönlendiren skill'ler.
- **[Frontend Check List]([https://github.com/GoogleChrome/modern-web-guidance-src](https://github.com/thedaviddias/Front-End-Checklist))** → Front-End Checklist is the open-source front-end quality system for humans and AI agents. It turns front-end best practices into a practical review workflow you can browse on the web, run through with MCP-compatible tools, or work through directly in this README.

## ✍️ Yazı, Pazarlama ve Görsel

- **[stop-slop](https://github.com/hardikpandya/stop-slop)** → Metinlerdeki tipik "AI kokan" kalıpları yakalayıp temizliyor. Yazılar daha doğal ve direkt çıkıyor.
- **[Marketing Skills](https://github.com/coreyhaines31/marketingskills)** → Agent'a pazarlama uzmanlığı kazandırıyor: dönüşüm optimizasyonu, copywriting, SEO, analitik, growth.
- **[Awesome GPT Image 2](https://github.com/freestylefly/awesome-gpt-image-2)** → GPT Image 2 için prompt ve örnek koleksiyonu; hazır yapılandırılmış prompt şablonları içeriyor.

## 🤖 Agent'lar ve Orkestrasyon

- **[Agency Agents](https://github.com/msitarzewski/agency-agents)** → Mühendislik, tasarım, pazarlama, satış, test ve güvenlik gibi alanlarda hazır uzman agent persona'ları. Claude Code'a kurulabilir ya da prompt referansı olarak kullanılabilir.
- **[Paperclip](https://github.com/paperclipai/paperclip)** → AI agent ekiplerini bir şirket gibi yönetmek için: org şeması, hedefler, görev takibi, onaylar ve bütçe tek dashboard'da.
- **[Claude Task Master](https://github.com/eyaltoledano/claude-task-master)** → Gereksinim dokümanını görevlere bölüyor, sıradaki görevi seçiyor. MCP veya CLI üzerinden çalışan AI destekli görev yönetimi.
- **[LLM Council](https://github.com/karpathy/llm-council)** → Karpathy'nin yan projesi. Bir soruyu birden fazla modele soruyor, modeller birbirinin cevabını anonim olarak puanlıyor, bir "başkan" model sonucu birleştiriyor.
- **[Awesome AI Agents](https://github.com/e2b-dev/awesome-ai-agents)** → Otonom AI agent'larının derlendiği büyük "awesome" listesi.

## 🔌 Öne Çıkan MCP Sunucuları

- **[Perplexity](https://github.com/perplexityai/modelcontextprotocol)** → Resmi Perplexity MCP. Claude'a canlı web araması, kaynaklı cevaplar ve derin araştırma yeteneği kazandırıyor. *(Perplexity API key gerekiyor.)*
- **[Firecrawl](https://github.com/firecrawl/firecrawl-mcp-server)** → Resmi Firecrawl MCP. Web sitelerini tarayıp, kazıyıp (scrape) agent'ın kullanabileceği temiz içeriğe çeviriyor.
- **[PostHog](https://posthog.com/docs/model-context-protocol/claude-code)** → Claude Code'dan doğrudan PostHog verine erişim: feature flag yönetimi, analitik sorguları, hata inceleme. Kurulum: `npx @posthog/wizard mcp add`
- **[Playwright](https://github.com/microsoft/playwright-mcp)** → Microsoft'tan. Claude'a gerçek bir tarayıcı veriyor; sayfaları ekran görüntüsü yerine erişilebilirlik ağacı üzerinden okuyor. E2E test ve otomasyon için ideal.
- **[Composio](https://docs.composio.dev/docs/claude-code-plugin)** → Tek MCP URL'si ile 1000+ uygulamaya (Gmail, Slack, GitHub vb.) bağlanma; kimlik doğrulama işini o hallediyor.

## 🚀 Canlıya Çıkmadan Önce Checklist

Bir projeyi production'a almadan önce mutlaka gözden geçirilmesi gerekenler:

**🔐 Güvenlik**
- [ ] Rate limiting (özellikle login, signup ve public API endpoint'leri)
- [ ] Secret'lar repoda değil; secrets manager / platform env ayarlarında
- [ ] Dev, staging ve production için ayrı key'ler
- [ ] CORS, security header'lar (CSP, HSTS) ve input validation
- [ ] Bağımlılıklarda bilinen açık taraması (`npm audit` vb.)

**⚙️ Konfigürasyon**
- [ ] Ortam değişkenleri uygulama açılırken doğrulanıyor (örn. Zod ile şema); eksikse uygulama hiç başlamıyor
- [ ] Staging ile production arasındaki farklar dokümante edildi

**🧯 Hata Yönetimi**
- [ ] Global error handler (kullanıcıya stack trace sızdırmadan)
- [ ] Geçici hatalar için retry ve timeout'lar
- [ ] Graceful shutdown (açık istekler ve DB bağlantıları düzgün kapanıyor)

**🗄️ Veri ve Altyapı**
- [ ] DB connection pool ayarlı
- [ ] Health check / readiness endpoint'i
- [ ] Otomatik yedekleme **ve** yedekten geri dönme test edildi
- [ ] Migration'lar geri alınabilir

**🚢 Deploy**
- [ ] Docker imajı (multi-stage, root olmayan kullanıcı)
- [ ] CI'da test + lint + build geçmeden deploy yok
- [ ] Rollback planı: bir önceki sürüme tek komutla dönülebiliyor

**📈 Gözlemlenebilirlik**
- [ ] Yapılandırılmış loglar
- [ ] Error tracking (Sentry, PostHog vb.)
- [ ] Uptime ve temel metrik alarmları

**Daha detaylı kaynaklar:**
- **[Gorrion Production Readiness Checklist](https://github.com/gorrion-io/production-readiness-checklist)** → Frontend, backend, güvenlik, monitoring, CI/CD ve deploy maddelerini kritik / olmalı / olsa iyi olur diye ayıran Markdown checklist.
- **[Microservice Production Readiness Checklist](https://github.com/kgoralski/microservice-production-readiness-checklist)** → Production'a güvenle deploy etmek için ilkeler; mikroservis, Kubernetes ve SRE odaklı.
- **[prodcheck](https://socket.dev/npm/package/prodcheck)** → Ship etmeden önce çalıştırılacak checklist'ler; repoya review skill'i olarak ya da Claude Code'a MCP olarak eklenebiliyor.
- **[Railway Production Readiness Checklist](https://docs.railway.com/platform/production-readiness-checklist)** → Performans, güvenilirlik ve gözlemlenebilirlik üzerine kısa ve pratik bir liste.

## 🌿 Git Öğren ve GitHub Hileleri

**Öğrenme yolu:**
1. **Git Essentials** → Temel komutlarla başla; takıldığın yerde Claude'a sorarak pratik yap.
2. **[Learn Git Branching](https://learngitbranching.js.org/)** → Tarayıcıda interaktif, görsel ve oyunlaştırılmış Git eğitimi. Branch, merge, rebase, cherry-pick'i commit ağacının canlı değiştiğini görerek öğreniyorsun.

**GitHub URL hileleri:**
- **[GitDiagram](https://gitdiagram.com)** → Herhangi bir GitHub URL'sinde `hub` yerine `diagram` yaz (`github.com/x/y` → `gitdiagram.com/x/y`), repo interaktif bir mimari diyagrama dönüşsün. Yabancı bir kod tabanını anlamanın en hızlı yolu. ([kaynak kod](https://github.com/ahmedkhaleel2004/gitdiagram))
- **[GitReverse](https://gitreverse.com)** → `github.com` yerine `gitreverse.com` yaz; repo, onu sıfırdan yeniden yaptırabileceğin bir AI prompt'una dönüşsün. Claude Code / Cursor'a proje tarif etmek için kullanışlı. ([kaynak kod](https://github.com/filiksyos/gitreverse))

## 📚 Kurslar

Kurslar, sırayla takip edilebilecek bir öğrenme yolu olarak dizildi. Her seviye bir öncekinin üzerine kuruluyor.
Konuya hakimsen ilgili seviyeyi atlayabilirsin.

### 1️⃣ Temeller — AI'ı anla
*Önce kavramlar: üretken AI nedir ve onunla nasıl verimli çalışılır.*

1. **[Google Skills – Introduction to Generative AI](https://www.skills.google/course_templates/536)** → Üretken AI nedir, klasik makine öğrenmesinden farkı ne, gerçek hayatta nerede kullanılıyor. ~45 dk, en hızlı giriş.
2. **[Claude Academy – AI Fluency: Framework & Foundations](https://academy.claude.com/courses/ai-fluency-framework-foundations)** → AI ile verimli ve güvenli çalışmanın 4 temel becerisi: görev devretme, net tarif etme, çıktıyı eleştirel değerlendirme, sorumluluk alma. Sonraki her kursta işine yarayacak alışkanlıklar.
3. *(Opsiyonel)* **[DeepLearning.AI – AI For Everyone](https://www.deeplearning.ai/courses/ai-for-everyone)** → Andrew Ng'den teknik olmayan bakış: AI projeleri nasıl yürür, şirketler AI'ı nasıl konumlar. Geliştiriciden çok PM / yönetici bakış açısı istersen.

### 2️⃣ Claude Code ile pratik
*Teoriyi bırakıp günlük işte kullanmaya başla.*

4. **[Claude Academy – Claude Code 101](https://academy.claude.com/courses/claude-code-101)** → Claude Code'a sıfırdan giriş: agent nasıl çalışır, kurulum, etkili prompt yazma, context yönetimi, değişiklikleri review etme. CLAUDE.md, subagent, skill, MCP ve hook'a ilk bakış.
5. **[DeepLearning.AI – Claude Code: A Highly Agentic Coding Assistant](https://www.deeplearning.ai/courses/claude-code-a-highly-agentic-coding-assistant)** → Anthropic ile hazırlanmış, daha uygulamalı devam kursu. Gerçek bir kod tabanında keşif, geliştirme, test, refactor ve debug; Playwright ve Figma MCP bağlantıları. ~2 saat.
6. 📖 *Yanında referans:* **[Claude How-To](https://github.com/luongnv89/claude-howto)** → Slash command, hafıza, skill, subagent, MCP, hook ve plugin'leri görsel ve örnekli anlatan rehber; kopyala-yapıştır şablonlarla. Baştan sona okumak yerine takıldıkça bak.

### 3️⃣ Claude'u genişlet
*Tek agent'tan çıkıp onu araçlarla ve yardımcı agent'larla güçlendir. README'deki skill ve MCP repolarının çoğu bu seviyeden sonra tam oturur.*

7. **[Claude Academy – Introduction to Subagents](https://academy.claude.com/courses/introduction-to-subagents)** → Karmaşık işleri paralel çalışan subagent'lara bölüp koordine etmek. `/agents` ile özel subagent oluşturma, ne zaman işe yaradıkları ve kaçınılması gereken anti-pattern'ler.
8. **[Claude Academy – Introduction to Model Context Protocol (MCP)](https://academy.claude.com/courses/introduction-to-model-context-protocol)** → Hazır MCP'leri kullanmaktan kendininkini yazmaya: Python ile MCP sunucusu ve istemcisi, tools / resources / prompts. Uygulamalı proje ve MCP Inspector ile test.

### 4️⃣ Kendi AI uygulamanı ve agent'ını yap
*Artık kullanıcı değil, geliştirici tarafındasın.*

9. **[Hugging Face – AI Agents Course](https://huggingface.co/learn/agents-course/unit1/introduction)** → Agent'ların "kaputun altı": LLM'in agent'ın beyni olarak rolü, araç kullanımı ve düşün → uygula → gözlemle döngüsü. smolagents ile ilk agent'ını yapıp yayınlıyorsun; sınavı geçene sertifika var.
10. **[Microsoft – Generative AI for Beginners (Türkçe)](https://github.com/microsoft/generative-ai-for-beginners/blob/main/translations/tr/README.md)** → 21 bağımsız ders: prompt engineering, chat/arama/görsel uygulamaları, RAG, agent'lar, fine-tuning. TypeScript örnekleri de var; ihtiyacın olan dersi seçip ilerleyebilirsin.
11. **[MongoDB University – AI Agents with MongoDB](https://learn.mongodb.com/courses/ai-agents-with-mongodb)** → Agent'ı gerçek uygulama verisine bağlamak: veritabanına güvenli okuma/yazma yapan tool'lar, orkestrasyon ve agent hafızası. Skill badge veriyor.

### 5️⃣ Ekip ölçeği
*Agent'ları tek başına değil, ekiple birlikte kullanmak.*

12. **[Claude Academy – Building Effective Human-Agent Teams](https://academy.claude.com/courses/building-effective-human-agent-teams)** → AI'ı kişisel asistandan ekibin ortak üyesine dönüştürmek: net roller, yazılı hedef, kademeli güven ve doğru bilgi erişimi. Kısa (~45 dk), teknik değil; ekipte AI kullanımını yönetecek olanlar için.

## 🧪 Denenecekler

- **[AI Job Search](https://github.com/ai-job-search-dev/ai-job-search)** → Claude Code'u iş başvuru asistanına çeviriyor: ilanları tarama ve değerlendirme, ilana özel CV ve ön yazı, mülakat hazırlığı, başvuru takibi. Tamamen yerelde çalışıyor.
- **[Mastra]([https://github.com/ai-job-search-dev/ai-job-search](https://github.com/mastra-ai/mastra))** → Mastra is a framework for building AI-powered applications and agents with a modern TypeScript stack.

## 🏕️ Boş Zamanda Bak

- **[HAS Prepper Disk](https://github.com/schematrix/HAS_Prepper_Disk)** → Raspberry Pi 5'i internetsiz çalışan bir bilgi kütüphanesine çeviriyor. Wikipedia, haritalar, tıbbi kaynaklar ve tamir rehberleri Pi'nin Wi-Fi'ı üzerinden yakındaki cihazlara sunuluyor.

---

⭐ Faydalı bulduysan repoya yıldız bırakmayı unutma!
