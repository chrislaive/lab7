<template>
    <div>
        <header>
            <div class="columns">
                <div class="column is-10">
                    <div id="Titulo">
                        <img src="lindavista.JPG" alt="">
                    </div>
                </div>
                
                <div class="column is-1">
                    <nuxt-link :to="switchLocalePath('es')" >[ Español <span class="icon"><img :src="require(`~/assets/flag-icons/es.svg`)"></span> ]</nuxt-link>
                </div>
                <div class="column is-1">
                    <nuxt-link :to="switchLocalePath('en')" >[ English <span class="icon"><img :src="require(`~/assets/flag-icons/en.svg`)"></span> ]</nuxt-link>
                </div>
            </div>
        </header>
        
        <div id="Central">
            <nav>
                <ul>
                    <li>{{$t('navbar.information')}}</li>
                    <li>{{$t('navbar.promotions')}}</li>
                    <li>{{$t('navbar.services')}}</li>
                    <li>{{$t('navbar.news')}}</li>
                    <li>{{$t('navbar.contact')}}</li>
                </ul>
            </nav>
            <section>
                <p>{{$t('section.news')}}</p>
                <div id="noticia">
                    <h2>{{$t('section.1.title')}}</h2>
                    <img class="fotonoticia" src="foto1.JPG" width="100" height="80"> 
                    <p class="textonoticia" v-html="$t('section.1.content')"></p>
                    <p><br></p>
                    
                </div>
                <div id="noticia">
                    <h2>{{$t('section.2.title')}}</h2>
                    <img class="fotonoticia" src="foto2.JPG" width="100" height="80" >
                    <p class="textonoticia" v-html="$t('section.2.content')"></p>
                    <p><br></p>
                    
                </div>
            </section>
            <aside>
                <ul class="anuncio">
                    <li class="anuncio"><img src="foto3.JPG" width="85" height="85" alt=""></li>
                    <li class="anuncio"><img src="foto4.JPG" width="85" height="85" alt=""></li>
                    <li class="anuncio"><img src="foto5.JPG" width="85" height="85" alt=""></li>
                    <li class="anuncio"><img src="foto6.JPG" width="85" height="85" alt=""></li>
                </ul>
            </aside>
            <div id="clear">
            
            </div>
        </div>
        <footer id="Pie">
            <p class="ppagina"><em>{{$t('footer')}}</em></p>
        </footer>

        <div id="certificado">
            <img src="valid-html401.gif" alt="HTML Válido" width="88" height="31">
            <img src="vcss.gif" alt="CSS Válido" width="88" height="31">
            <img src="wcag1AAA.gif" alt="Icono de conformidad con el Nivel Triple-A, 
                de las Directrices de Accesibilidad para el 
                Contenido Web 1.0 del W3C-WAI" width="88" height="31">
        </div>
    </div>
</template>
