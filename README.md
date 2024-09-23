<h2> ISAMAYA </h2>
<p>In this project main focus was on changing media order to create tiled galleries on the PDPs and display product swatches on hover.</br>
To achieve this I've adjusted two code snippets.</p>
<ol>
  <li>Hover media re-assign - <a href ="https://github.com/lifelesshaze/palo-alto/blob/1639ef6071403c62dfdf4ed2e8a835cb1edceb58/product-grid-item.liquid"> product-grid-item.liquid </a> 
  <blockquote>I used this code snippet to change hover media for product cards in grids (collection pages, featured collection widget, etc.)</br>
  It runs on two conditions: </br> 
    <ul>
      <li>whether product has more or less than 3 media uploaded;</li>
      <li>whether product was assigned specific template;</li>
    </ul> 
  In case none of these conditions apply, default media order is used.</blockquote></li>
  <li>Swap media on PDPs - <a href = "https://github.com/lifelesshaze/palo-alto/blob/1639ef6071403c62dfdf4ed2e8a835cb1edceb58/product.liquid">product.liquid</a>
  <blockquote>I used this code snippet to change media order in galleries on PDPs.</br>
  It checks product template, title and quantity of uploaded media and swaps first and second images, keeping rest of the media intact.</li>
</ol>
</br>
</br>
<h2>VOLZHENKA</h2>
<h3>Footer adjustments</h3> </br>
<p>It was necessary to completely change the look of the footer to align with overall brand's style. </br>
  They were looking for clean and minimalistic look. To do so I've created new snippet to render localization block, adjusted schema for the footer section, slightly changed code for footer snippet and, finally, styled it with CSS.</p>
<ol>
  <li>Create new snippet - <a href = "https://github.com/lifelesshaze/palo-alto/blob/935305a88aca04b845d53b4d3af2ff210b6e9826/snippet-localization.liquid"> snippet-localization.liquid </a>
    <blockquote>This snippet creates new localization block for main footer instead of displaying it in subfooter</blockquote>
  </li>
  <li> Adjust schema for existing footer section - <a href = "https://github.com/lifelesshaze/palo-alto/blob/935305a88aca04b845d53b4d3af2ff210b6e9826/section-footer.liquid"> section-footer.liquid </a>
    <blockquote>Added standard settings for our new localization block: such as text alignment and block width</blockquote>
  </li>
  <li> Adjust footer snippet - <a href = "https://github.com/lifelesshaze/palo-alto/blob/935305a88aca04b845d53b4d3af2ff210b6e9826/snippet-footer.liquid"> snippet-footer.liquid </a>
    <blockquote>Condition to check whether localization block is added in the theme, if yes - it's being rendered.</blockquote>
  </li>
  <li> Style updated footer - <a href = "https://github.com/lifelesshaze/palo-alto/blob/935305a88aca04b845d53b4d3af2ff210b6e9826/custom_theme.css"> custom_theme.css </a>
    <blockquote>Cutomised paddings, line-height, margins and menu section width. Also changed type for displaying menu block.</blockquote>
  </li>
</ol>
