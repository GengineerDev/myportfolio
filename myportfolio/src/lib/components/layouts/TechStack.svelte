<script>
	import Tag from "../elements/Tag.svelte";
</script>

<style>
    .tech-stack {
        padding: 0 120px;
        margin-top: 64px;
    }
    
    .tech-stack-container {
        margin: 16px 0;
        display: flex;
        justify-content: center;
        align-items: center;
        align-content: center;
        gap: 12px;
        align-self: stretch;
        flex-wrap: wrap;
    }

    .tech-stack h2 {
        margin-bottom: 16px;
    }

    .tech-stack-card-row {
        display: flex;
        gap: 16px;
        align-items: center;
        justify-content: space-around;
    }
</style>

<div class="tech-stack">
    <center>
        <h2 class="gradient-text-background">TECH STACK</h2>
    </center>
    <div class="tech-stack-container">
        <Tag>ALL</Tag>
        <Tag>Frontend Development</Tag>
        <Tag>Backend Development</Tag>
        <Tag>Mobile App Development</Tag>
        <Tag>General Programming</Tag>
        <Tag>Machine Learning</Tag>
        <Tag>Toolkit</Tag>
    </div>
    <div class="tech-stack-card-row">
        <img src="/images/tech-stack/HTML.svg" alt="HTML" />
        <img src="/images/tech-stack/CSS.svg" alt="CSS" />
        <img src="/images/tech-stack/SaSS.svg" alt="SaSS" />
        <img src="/images/tech-stack/JS.svg" alt="JS" />
        <img src="/images/tech-stack/ReactJS.svg" alt="ReactJS" />
    </div>
    <div class="tech-stack-card-row">
        <img src="/images/tech-stack/SvelteJS.svg" alt="SvelteJS" />
        <img src="/images/tech-stack/MongoDB.svg" alt="MongoDB" />
        <img src="/images/tech-stack/NodeJS.svg" alt="NodeJS" />
        <img src="/images/tech-stack/ExpressJS.svg" alt="ExpressJS" />
        <img src="/images/tech-stack/Django.svg" alt="Django" />        
    </div>
    <div class="tech-stack-card-row">
        <img src="/images/tech-stack/Java.svg" alt="Java" />
        <img src="/images/tech-stack/Python.svg" alt="Python" />
        <img src="/images/tech-stack/C.svg" alt="C" />
        <img src="/images/tech-stack/C-plus-plus.svg" alt="C-plus-plus" />
        <img src="/images/tech-stack/C-sharp.svg" alt="C-sharp" />
        <img src="/images/tech-stack/TensorFlow.svg" alt="TensorFlow" />        
    </div>
    <div class="tech-stack-card-row">
        <img src="/images/tech-stack/NumPy.svg" alt="NumPy" />   
        <img src="/images/tech-stack/Flutter.svg" alt="Flutter" />     
        <img src="/images/tech-stack/Dart.svg" alt="Dart" />
        <img src="/images/tech-stack/VS Code.svg" alt="VS Code" />  
        <img src="/images/tech-stack/GitHub.svg" alt="GitHub" />      
    </div>
    <div class="tech-stack-container">        
        <img src="/images/tech-stack/Terminal.svg" alt="Terminal" />
        <img src="/images/tech-stack/WordPress.svg" alt="WordPress" />
        <img src="/images/tech-stack/Figma.svg" alt="Figma" />
    </div>    
</div>
