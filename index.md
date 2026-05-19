layout: homepage<!-- ====== 加入高级交互流水线动画 Demo ====== -->
<div class="ai-pipeline-wrapper">
  <div class="pipeline-title">Research Pipeline</div>
  <svg class="pipeline-svg" viewBox="0 0 650 180">
    <!-- 轨道线 -->
    <path class="track-line-light" d="M 90 60 L 260 60" />
    <path class="track-line-light" d="M 390 60 L 560 60" />
    
    <!-- 流动光线 -->
    <path class="flow-line-light" d="M 90 60 L 260 60" />
    <path class="flow-line-light" d="M 390 60 L 560 60" style="animation-delay: 1.5s; stroke: #AF52DE;" />

    <!-- 流动字符 -->
    <text x="130" y="56" class="data-stream-light" style="animation-delay: 0.5s;">A_C_G_T...seq_01</text>
    <text x="430" y="56" class="data-stream-light" style="animation-delay: 2s; fill: #AF52DE;">gen_struct_72</text>

    <!-- 左侧：Omics (苹果绿) -->
    <g transform="translate(90, 60)">
      <circle cx="-18" cy="-15" r="3" fill="#34C759" opacity="0.4"><animate attributeName="opacity" values="0.4;0.8;0.4" dur="2s" infinite delay="0.1s"/></circle>
      <circle cx="-8" cy="-25" r="2.5" fill="#34C759" opacity="0.3"><animate attributeName="opacity" values="0.3;0.7;0.3" dur="2.2s" infinite delay="0.3s"/></circle>
      <circle cx="8" cy="-12" r="4.5" fill="#34C759" opacity="0.6"><animate attributeName="opacity" values="0.6;1;0.6" dur="1.8s" infinite delay="0.5s"/></circle>
      <circle cx="-25" cy="8" r="3" fill="#34C759" opacity="0.3"><animate attributeName="opacity" values="0.3;0.8;0.3" dur="2.5s" infinite delay="0.2s"/></circle>
      <circle cx="-8" cy="20" r="4" fill="#34C759" opacity="0.5"><animate attributeName="opacity" values="0.5;0.9;0.5" dur="2s" infinite delay="0.4s"/></circle>
      <circle cx="15" cy="10" r="2" fill="#34C759" opacity="0.4"><animate attributeName="opacity" values="0.4;0.8;0.4" dur="2.1s" infinite delay="0.6s"/></circle>
      <circle cx="0" cy="0" r="5" fill="#34C759" /> 
      <text y="45" class="node-text-light">Omics Targets</text>
      <text y="58" class="tech-label-light">scOmics-seq / Data Input</text>
    </g>

    <!-- 中央：AI Engine (苹果蓝) -->
    <g transform="translate(325, 60)">
      <g transform="rotate(45)"><path class="ai-kernel-light" d="M -25 0 Q 0 -10 25 0 Q 0 10 -25 0 Z L 0 -15 L 0 15 Z" style="animation-delay: 0s;" /></g>
      <g transform="rotate(135)"><path class="ai-kernel-light" d="M -20 0 Q 0 -8 20 0 Q 0 8 -20 0 Z L 0 -12 L 0 12 Z" style="animation-delay: 1.3s;" /></g>
      <g transform="translate(-50, -50)">
        <path class="weight-line-light" d="M 0 0 L 33 0 L 33 33 L 0 33 Z" />
        <path class="weight-line-light" d="M 33 0 L 66 0 L 66 33 L 33 33 Z" />
        <path class="weight-line-light" d="M 66 0 L 99 0 L 99 33 L 66 33 Z" />
        <path class="weight-line-light" d="M 0 33 L 33 33 L 33 66 L 0 66 Z" />
        <path class="weight-line-light" d="M 33 33 L 66 33 L 66 66 L 33 66 Z" />
        <path class="weight-line-light" d="M 66 33 L 99 33 L 99 66 L 66 66 Z" />
        <path class="weight-line-light" d="M 0 66 L 33 66 L 33 99 L 0 99 Z" />
        <path class="weight-line-light" d="M 33 66 L 66 66 L 66 99 L 33 99 Z" />
        <path class="weight-line-light" d="M 66 66 L 99 66 L 99 99 L 66 99 Z" />
        <circle cx="0" cy="0" r="2.5" class="network-node-light" style="animation-delay: 0.2s;" />
        <circle cx="33" cy="0" r="2.5" class="network-node-light" style="animation-delay: 0.5s;" />
        <circle cx="66" cy="0" r="2.5" class="network-node-light" style="animation-delay: 0.1s;" />
        <circle cx="99" cy="0" r="2.5" class="network-node-light" style="animation-delay: 0.4s;" />
        <circle cx="33" cy="33" r="2.5" class="network-node-light" style="animation-delay: 0.3s;" />
        <circle cx="66" cy="33" r="2.5" class="network-node-light" style="animation-delay: 0.7s;" />
        <circle cx="33" cy="66" r="2.5" class="network-node-light" style="animation-delay: 0.8s;" />
        <circle cx="66" cy="66" r="2.5" class="network-node-light" style="animation-delay: 0.1s;" />
        <circle cx="99" cy="99" r="2.5" class="network-node-light" style="animation-delay: 0.2s;" />
      </g>
      <text y="-55" class="tech-label-light" style="fill:#007AFF; font-weight: 600;">Transformer Core</text>
      <text y="65" class="node-text-light">Generative AI Engine</text>
      <text y="78" class="tech-label-light">Latent Space Mapping</text>
    </g>

    <!-- 右侧：De Novo Design (苹果紫) -->
    <g transform="translate(560, 60)">
      <polygon points="0,-25 21,-12 21,12 0,25 -21,12 -21,-12" fill="none" stroke="#AF52DE" stroke-width="2" stroke-linejoin="round" />
      <line x1="21" y1="-12" x2="35" y2="-21" stroke="#AF52DE" stroke-width="2" stroke-linecap="round" />
      <circle cx="38" cy="-23" r="4.5" fill="#AF52DE" />
      <line x1="-10" y1="6" x2="10" y2="-6" stroke="#AF52DE" stroke-width="1" opacity="0.5" />
      <text y="45" class="node-text-light">De Novo Design</text>
      <text y="58" class="tech-label-light">Optimized Structures</text>
    </g>
  </svg>
</div>
<!-- ====== 动画 Demo 结束 ====== -->
<article class="feature-row">
  <div class="feature-meta">
    <span>NeurIPS</span>
    <span>2024</span>
  </div>
  <div class="feature-copy">
    <h3>A versatile informative diffusion model for single-cell ATAC-seq data generation and analysis</h3>
    <p>A generative framework for chromatin accessibility data, developed during my visiting scholar work with the Kellis Lab.</p>
  </div>
</article>

<article class="feature-row">
  <div class="feature-meta">
    <span>Nature Communications</span>
    <span>2024</span>
  </div>
  <div class="feature-copy">
    <h3>A dual diffusion model enables 3D binding bioactive molecule generation and lead optimization</h3>
    <p>Target-pocket-conditioned molecular generation for structure-aware lead optimization.</p>
    <div class="link-row">
      <a href="https://www.nature.com/articles/s41467-024-46569-1" target="_blank" rel="noopener">Paper</a>
      <a href="https://github.com/Layne-Huang/PMDM/tree/main" target="_blank" rel="noopener">Code</a>
    </div>
  </div>
</article>
