<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600&display=swap');
*{box-sizing:border-box;margin:0;padding:0}
body{background:#b0f6c0;font-family:'Montserrat',sans-serif}
.wrap{max-width:860px;margin:0 auto;background:#b0f6c0;padding-bottom:3rem}
.hero{background:#1a4d0a;padding:2.5rem 3rem;border-radius:0 0 32px 32px;margin-bottom:2rem}
.hero-tag{display:inline-flex;align-items:center;gap:6px;background:#143d07;color:#7dd87a;font-size:13px;font-weight:500;padding:5px 14px;border-radius:20px;margin-bottom:14px}
.hero h1{color:#fff;font-size:36px;font-weight:600;line-height:1.2;margin-bottom:10px}
.hero p{color:#a0d87a;font-size:15px;line-height:1.6;max-width:560px}
.content{padding:0 2rem}
.section-label{font-size:11px;color:#1a4d0a;font-weight:600;text-transform:uppercase;letter-spacing:0.09em;margin-bottom:12px;opacity:0.6}
.faq-list{display:flex;flex-direction:column;gap:10px}
.faq-item{background:#fff;border:none;border-radius:16px;overflow:hidden;box-shadow:0 1px 6px rgba(26,77,10,0.08)}
.faq-btn{width:100%;background:none;border:none;cursor:pointer;display:flex;align-items:center;gap:14px;padding:18px 22px;text-align:left;font-family:'Montserrat',sans-serif}
.faq-icon{width:34px;height:34px;min-width:34px;border-radius:50%;background:#e2fce8;display:flex;align-items:center;justify-content:center;transition:background 0.2s}
.faq-item.open .faq-icon{background:#1a4d0a}
.faq-icon i{font-size:16px;color:#1a4d0a;transition:color 0.2s}
.faq-item.open .faq-icon i{color:#fff}
.faq-q{font-size:15px;font-weight:500;color:#1a4d0a;line-height:1.4;flex:1}
.chevron{font-size:18px;color:#1a4d0a;transition:transform 0.25s;min-width:18px;opacity:0.7}
.faq-item.open .chevron{transform:rotate(180deg);opacity:1}
.faq-body{max-height:0;overflow:hidden;transition:max-height 0.35s ease}
.faq-body.open{max-height:600px;padding:0 22px 20px}
.faq-body p{font-size:14px;color:#1a4d0a;line-height:1.7;opacity:0.85}
.faq-body ul{margin:10px 0 0 4px;display:flex;flex-direction:column;gap:8px}
.faq-body li{font-size:14px;color:#1a4d0a;line-height:1.6;display:flex;gap:10px;opacity:0.85}
.faq-body li::before{content:"–";color:#1a4d0a;flex-shrink:0;opacity:0.5}
.faq-body strong{color:#1a4d0a;font-weight:600;opacity:1}
.faq-body a{color:#1a4d0a;font-weight:500}
.script-box{background:#e2fce8;border-left:3px solid #1a4d0a;border-radius:0 10px 10px 0;padding:12px 16px;margin-top:12px;font-size:14px;color:#1a4d0a;line-height:1.7;font-style:italic}
.copy-btn{display:inline-flex;align-items:center;gap:6px;margin-top:10px;background:none;border:1px solid #1a4d0a;border-radius:20px;padding:6px 14px;font-size:13px;color:#1a4d0a;cursor:pointer;font-family:'Montserrat',sans-serif;transition:background 0.2s}
.copy-btn:hover{background:#e2fce8}
.copy-btn i{font-size:14px}
.alert-box{background:#e2fce8;border-left:3px solid #1a4d0a;border-radius:0 10px 10px 0;padding:12px 16px;margin-top:12px;font-size:14px;color:#1a4d0a;line-height:1.7}
.alert-box strong{color:#1a4d0a;font-size:16px}
.divider{height:1px;background:#1a4d0a;opacity:0.15;margin:2.5rem 2rem 1.5rem}
.footer{text-align:center;padding:0 2rem 1.5rem}
.footer img{height:52px;width:auto;display:inline-block}
</style>

<div class="wrap">
  <div class="hero">
    <div class="hero-tag"><i class="ti ti-refresh" aria-hidden="true"></i> Virada de sistema — este domingo</div>
    <h1>FAQ Colaboradores<br>Atualização de Sistema</h1>
    <p>Alinhamento de equipe e orientações para o atendimento durante a transição.</p>
  </div>

  <div class="content">
    <div class="section-label">Perguntas frequentes</div>
    <div class="faq-list" id="faq">

      <div class="faq-item" data-idx="0">
        <button class="faq-btn" onclick="toggle(0)" aria-expanded="false">
          <div class="faq-icon"><i class="ti ti-help" aria-hidden="true"></i></div>
          <span class="faq-q">Por que o sistema está mudando?</span>
          <i class="ti ti-chevron-down chevron" aria-hidden="true"></i>
        </button>
        <div class="faq-body" id="body-0">
          <p>A atualização faz parte do plano de melhoria contínua. O novo sistema trará mais <strong>eficiência para a rotina interna</strong> e agilidade no atendimento ao cliente a longo prazo.</p>
        </div>
      </div>

      <div class="faq-item" data-idx="1">
        <button class="faq-btn" onclick="toggle(1)" aria-expanded="false">
          <div class="faq-icon"><i class="ti ti-alert-circle" aria-hidden="true"></i></div>
          <span class="faq-q">Qual será o impacto direto na operação?</span>
          <i class="ti ti-chevron-down chevron" aria-hidden="true"></i>
        </button>
        <div class="faq-body" id="body-1">
          <ul>
            <li><span><strong>Logística e Recebimento:</strong> Recebimento de amostras funciona normalmente. Sem alteração no fluxo de coleta e entrega de materiais.</span></li>
            <li><span><strong>Unidade Indianópolis:</strong> Excepcionalmente fechada neste domingo devido à atualização.</span></li>
            <li><span><strong>Liberação de Laudos:</strong> Sistema pode apresentar instabilidades e lentidão, gerando atrasos nos resultados de exames.</span></li>
          </ul>
        </div>
      </div>

      <div class="faq-item" data-idx="2">
        <button class="faq-btn" onclick="toggle(2)" aria-expanded="false">
          <div class="faq-icon"><i class="ti ti-user" aria-hidden="true"></i></div>
          <span class="faq-q">O que falar para o tutor (B2C) se reclamar do atraso no exame?</span>
          <i class="ti ti-chevron-down chevron" aria-hidden="true"></i>
        </button>
        <div class="faq-body" id="body-2">
          <p>Seja empático e transparente. Use o argumento abaixo:</p>
          <div class="script-box" id="script-b2c">"Pedimos desculpas pelo tempo de espera. Estamos passando por uma atualização importante em nosso sistema hoje para melhorar a entrega dos nossos serviços. Nossa equipe técnica já está trabalhando para liberar o seu resultado o mais rápido possível."</div>
          <button class="copy-btn" onclick="copyText('script-b2c',this)"><i class="ti ti-copy" aria-hidden="true"></i> Copiar script</button>
        </div>
      </div>

      <div class="faq-item" data-idx="3">
        <button class="faq-btn" onclick="toggle(3)" aria-expanded="false">
          <div class="faq-icon"><i class="ti ti-stethoscope" aria-hidden="true"></i></div>
          <span class="faq-q">O que falar para os parceiros veterinários (B2B)?</span>
          <i class="ti ti-chevron-down chevron" aria-hidden="true"></i>
        </button>
        <div class="faq-body" id="body-3">
          <p>Reforce que o recebimento das amostras segue normal e que a equipe técnica está empenhada em reduzir o impacto nos laudos:</p>
          <div class="script-box" id="script-b2b">"Doutor(a), a nossa logística de amostras segue rodando normalmente. Contudo, devido a uma virada de sistema programada para melhorias na plataforma, a liberação de alguns laudos pode sofrer um leve atraso. Agradecemos muito a parceria e compreensão."</div>
          <button class="copy-btn" onclick="copyText('script-b2b',this)"><i class="ti ti-copy" aria-hidden="true"></i> Copiar script</button>
        </div>
      </div>

      <div class="faq-item" data-idx="4">
        <button class="faq-btn" onclick="toggle(4)" aria-expanded="false">
          <div class="faq-icon"><i class="ti ti-map-pin" aria-hidden="true"></i></div>
          <span class="faq-q">Como proceder com clientes que buscarem atendimento na Unidade Indianópolis?</span>
          <i class="ti ti-chevron-down chevron" aria-hidden="true"></i>
        </button>
        <div class="faq-body" id="body-4">
          <p>A unidade estará <strong>fechada neste domingo</strong> devido à atualização. Oriente o cliente a realizar o agendamento ou comparecer para exames <strong>a partir de segunda-feira</strong>, quando a unidade retomará o funcionamento normal já com o novo sistema.</p>
        </div>
      </div>

      <div class="faq-item" data-idx="5">
        <button class="faq-btn" onclick="toggle(5)" aria-expanded="false">
          <div class="faq-icon"><i class="ti ti-login" aria-hidden="true"></i></div>
          <span class="faq-q">Como os colaboradores vão acessar o novo sistema?</span>
          <i class="ti ti-chevron-down chevron" aria-hidden="true"></i>
        </button>
        <div class="faq-body" id="body-5">
          <p>Para acessar a nova plataforma, siga as instruções abaixo:</p>
          <p style="margin-top:10px"><strong>Link de acesso:</strong> <a href="https://provet-login.pixeonkorus.com/" target="_blank">https://provet-login.pixeonkorus.com/</a></p>
          <p style="margin-top:10px">Na tela de login, preencha os campos da seguinte forma:</p>
          <ul style="margin-top:8px">
            <li><span><strong>Domínio:</strong> provet</span></li>
            <li><span><strong>Login:</strong> O mesmo usuário que você já utiliza no Pleres</span></li>
            <li><span><strong>Senha:</strong> A mesma senha que você já utiliza no Pleres</span></li>
          </ul>
        </div>
      </div>

      <div class="faq-item" data-idx="6">
        <button class="faq-btn" onclick="toggle(6)" aria-expanded="false">
          <div class="faq-icon"><i class="ti ti-tool" aria-hidden="true"></i></div>
          <span class="faq-q">Tive um problema técnico crítico durante o plantão. Quem devo acionar?</span>
          <i class="ti ti-chevron-down chevron" aria-hidden="true"></i>
        </button>
        <div class="faq-body" id="body-6">
          <p>Em caso de travamentos ou dúvidas técnicas impeditivas, acione imediatamente o plantão de TI/Suporte pelo canal oficial:</p>
          <div class="alert-box"><strong>Ramal *100</strong> — canal oficial de suporte durante a virada de sistema.</div>
        </div>
      </div>

    </div>

    <div class="divider"></div>
    <div class="footer">
      <img src="https://d335luupugsy2.cloudfront.net/cms/files/57798/1774291311/$0v9mfq08cfuj" alt="Provet"/>
    </div>
  </div>
</div>

<script>
function toggle(idx){
  var item=document.querySelector('[data-idx="'+idx+'"]');
  var body=document.getElementById('body-'+idx);
  var btn=item.querySelector('.faq-btn');
  var isOpen=item.classList.contains('open');
  document.querySelectorAll('.faq-item').forEach(function(el){
    el.classList.remove('open');
    el.querySelector('.faq-body').classList.remove('open');
    el.querySelector('.faq-btn').setAttribute('aria-expanded','false');
  });
  if(!isOpen){
    item.classList.add('open');
    body.classList.add('open');
    btn.setAttribute('aria-expanded','true');
  }
}
function copyText(id,btn){
  var txt=document.getElementById(id).innerText.replace(/^"|"$/g,'');
  navigator.clipboard.writeText(txt).then(function(){
    btn.innerHTML='<i class="ti ti-check" aria-hidden="true"></i> Copiado!';
    setTimeout(function(){btn.innerHTML='<i class="ti ti-copy" aria-hidden="true"></i> Copiar script';},2000);
  });
}
</script>
