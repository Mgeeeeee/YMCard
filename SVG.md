<svg id="note" xmlns="http://www.w3.org/2000/svg" width="1080" height="1920" viewBox="0 0 1080 1920">
  <defs>
    <style>
      #note .gaegu { color: #333; filter: url(#text-on-paper); position: relative; height: 100%; } #note .title { font-size: 70px; font-weight: 700; text-align: center; margin-bottom: 80px; } #note .body { font-size: 55px; line-height: 1.6; margin-bottom: 100px; text-align: left; } #note .summary { font-size: 55px; font-style: italic; text-align: center; color: #444; position: absolute; bottom: 0; left: 0; width: 100%;  }
    </style>
    <clipPath id="frame">
      <rect x="0" y="0" width="1080" height="1920"/>
    </clipPath>
    <filter id="paper-bg" x="0" y="0" width="1080" height="1920" color-interpolation-filters="sRGB">
      <feTurbulence type="fractalNoise" baseFrequency="0.05" numOctaves="4" seed="3" result="NOISE"/>
      <feDiffuseLighting in="NOISE" lighting-color="white" surfaceScale="1.8" result="LIGHT">
        <feDistantLight azimuth="45" elevation="60"/>
      </feDiffuseLighting>
      <feFlood flood-color="#fff" result="BASE"/>
      <feBlend in="BASE" in2="LIGHT" mode="multiply" result="PAPER"/>
    </filter>
    <filter id="text-on-paper" x="-6%" y="-40%" width="112%" height="180%" color-interpolation-filters="sRGB">
      <feTurbulence type="fractalNoise" baseFrequency="0.05" numOctaves="4" seed="3" result="NOISE"/>
      <feDiffuseLighting in="NOISE" lighting-color="white" surfaceScale="1.8" result="LIGHT"/>
      <feGaussianBlur in="SourceGraphic" stdDeviation="0.4" result="SOFT"/>
      <feDisplacementMap in="SOFT" in2="NOISE" xChannelSelector="R" yChannelSelector="G" scale="8" result="WARP"/>
      <feComponentTransfer in="LIGHT" result="LIGHT_TONE">
        <feFuncR type="linear" slope="0.9"/>
        <feFuncG type="linear" slope="0.9"/>
        <feFuncB type="linear" slope="0.9"/>
      </feComponentTransfer>
      <feBlend in="WARP" in2="LIGHT_TONE" mode="multiply"/>
    </filter>
    <symbol id="leaf" viewBox="-40 -20 80 40">
      <path d="M-30,0 C-20,-15 20,-15 30,0 C20,15 -20,15 -30,0Z" fill="#6b8f57" fill-opacity="0.35" stroke="#4f6d3f" stroke-opacity="0.45" stroke-width="2"/>
      <path d="M-28,0 C-10,-5 10,-5 28,0" fill="none" stroke="#4f6d3f" stroke-opacity="0.45" stroke-width="1.5"/>
    </symbol>
  </defs>
  <rect x="0" y="0" width="1080" height="1920" filter="url(#paper-bg)"/>
  <g filter="url(#text-on-paper)">
    <use href="#leaf" transform="translate(100,400) scale(1.00) rotate(10)"/>
    <use href="#leaf" transform="translate(100,500) scale(0.75) rotate(-22)"/>
    <use href="#leaf" transform="translate(400,100) scale(0.55) rotate(30)"/>
    <use href="#leaf" transform="translate(120,120) scale(0.1) rotate(20)"/>
    <use href="#leaf" transform="translate(800,100) scale(0.15) rotate(-25)"/>
  </g>
  <g clip-path="url(#frame)">
    <foreignObject x="120" y="180" width="840" height="1500">
      <div xmlns="http://www.w3.org/1999/xhtml" class="gaegu">
        <div class="title">
          {故事标题}
        </div>
        <div class="body">
          {故事正文}
        </div>
        <div class="summary">
          {故事总结}
        </div>
      </div>
    </foreignObject>
  </g>
  <g transform="translate(540,1830)" fill="#333" filter="url(#text-on-paper)">
    <g transform="translate(-50,-28.5)">
      <svg width="100" height="57" viewBox="0 0 24.4 14">
        <path d="M1.88672 0C3.45875 0.000168653 4.7334 1.27461 4.7334 2.84668V9.7998C4.7334 10.8307 5.56966 11.667 6.60059 11.667C7.63124 11.6667 8.4668 10.8305 8.4668 9.7998V4.92285C8.46706 2.20399 10.6717 0 13.3906 0C16.1093 0.000341475 18.3132 2.2042 18.3135 4.92285V14H16.2607C15.23 14 14.3938 13.1645 14.3936 12.1338V4.71289C14.3933 3.39877 13.3278 2.33319 12.0137 2.33301C10.6994 2.33301 9.63403 3.39866 9.63379 4.71289V9.68359C9.63365 12.0673 7.701 13.9996 5.31738 14C2.93344 14 1.00014 12.0675 1 9.68359V0H1.88672ZM19.9004 2.33301C22.191 2.33321 24.0753 4.07095 24.3086 6.2998C24.3246 6.45314 24.333 6.60902 24.333 6.7666V14H22.6768C21.646 14 20.8098 13.1645 20.8096 12.1338V6.2998C20.8095 4.73481 20.0524 3.34138 18.9102 2.44434C18.9291 2.44001 18.9487 2.43572 18.9678 2.43164C19.2683 2.36734 19.5807 2.33301 19.9004 2.33301Z"/>
      </svg>
    </g>
  </g>
</svg>
