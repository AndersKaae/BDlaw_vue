<template>
    <div class="container">
        <div class="content">
            <div class="menu">
                <div class="exitbutton">X</div>
            </div>
            <div class="textfield">
                <h1 class="cover-heading">Lovpligtige Oplysninger</h1>
                <p class="lead">Vi følger Advokatsamfundets regler for advokatetik og god advokatskik. Vores rådgivning er baseret på dansk ret, og vi er underlagt reglerne om forebyggelse af hvidvask.<br></p>
                <p class="lead">Alle vores advokater:</p>
                <p class="lead">er beskikket som advokat af Justitsministeriet i Danmark</p>
                <p class="lead">er medlemmer af Advokatsamfundet</p>
                <p class="lead">har tegnet ansvarsforsikring og stillet garanti efter de af Advokatsamfundet fastsatte regler. Ansvarsforsikringen dækker al advokatvirksomhed, uanset hvor advokatvirksomheden udøves.</p>
                <p class="lead">er medlem af Danske Advokater</p>
                <p class="lead">anvender ikke aftaleklausuler om lovvalg og/eller værneting, medmindre dette aftales med klienten</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
.container{
    display: block;
    position: absolute;
    background-color: rgb(135, 42, 185);
    border: solid;
    border-color: rgb(69, 1, 63);
    width: 500px;
    height: 600px;
    margin-top: 8%;
    margin-left: 20%;
    display: flex;
    align-items: center;
}

.content{
    height: 98%;
    width: 98%;
    margin-bottom: 100px;
    border: solid;
    border-color: rgb(69, 1, 63);
    background-color: rgb(185, 42, 175);
    margin: auto;
    
}
.menu{
    background-color: rgb(135, 42, 185);
    margin-top: -4px;
    height: 40px;
    margin-left: -2px;
    margin-right: -2px;
    border-bottom: solid;
    border-color: rgb(69, 1, 63);
}

.exitbutton{
    user-select: none;
    width: 40px;
    float: right;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 27px;
    text-align: center;
    padding-top: 3px;
    padding-bottom: 4px;
    cursor: pointer;
}

.textfield{
    padding-left: 10px;
    font-family:Arial, Helvetica, sans-serif
}
</style>