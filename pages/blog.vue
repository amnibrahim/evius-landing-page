<template>
  <section class="container">
    <div id="wrap">
      <div id="leftPane" class="bgdarkBlue">
        <div id="stickyPane">
          <p id="title">Lorem ipsum dolor amet seitan beard</p>
          <p class="meta">evius</p>
          <p class="meta">01-10-2018</p>
        </div>
      </div>
      <div id="rightPane" class="bgwhite">
        <div id="mainText">
          <p>
            Lorem ipsum dolor amet seitan beard
          </p>
          <p>
            Lorem ipsum dolor amet seitan beard pug bushwick chillwave sartorial, wolf woke drinking vinegar. Literally iPhone marfa palo santo chillwave subway tile yr unicorn ennui distillery +1. Cold-pressed poutine meh, chia iPhone glossier chambray brooklyn. Single-origin coffee fingerstache normcore knausgaard you probably haven't heard of them taxidermy, wolf prism raw denim letterpress YOLO.
          </p>
          <ul>
            <li>Adjusted rand index</li>
            <li>Mutual information based scoring</li>
            <li>Homogeneity, completeness and v-measure</li>
          </ul>
          <p>
            Plaid irony blog kogi unicorn slow-carb street art gochujang salvia. Pickled meditation polaroid fixie. Single-origin coffee aesthetic viral irony. PBR&B lomo YOLO cred roof party prism before they sold out knausgaard ramps disrupt chillwave.
          </p>
          <img src="~/assets/img/uu3.png">
          <p>
            Fingerstache wolf celiac, asymmetrical messenger bag trust fund YOLO normcore. Tumeric wolf bitters chicharrones meh. Forage gochujang wayfarers church-key, polaroid sustainable jianbing la croix. Hella vice live-edge gastropub, roof party twee fam portland gluten-free try-hard small batch. Yuccie copper mug activated charcoal banjo food truck asymmetrical cold-pressed snackwave chia direct trade raw denim chicharrones kale chips plaid. 3 wolf moon enamel pin echo park, cray etsy artisan slow-carb kogi +1 8-bit cronut gastropub stumptown.
          </p>
          <p>
            Pok pok franzen activated charcoal drinking vinegar church-key DIY deep v PBR&B semiotics vape kombucha cardigan. Pitchfork narwhal deep v mlkshk kogi craft beer marfa readymade roof party intelligentsia vinyl quinoa fam vexillologist. Brunch raw denim hoodie forage tote bag chia, hammock XOXO helvetica cred air plant art party. Yr celiac chia shaman etsy meditation, shoreditch palo santo adaptogen slow-carb pickled lo-fi pok pok sartorial biodiesel. Kale chips banjo shaman yr.
          </p>
          <p>
            Brunch twee la croix kinfolk kickstarter hammock godard tilde etsy. Crucifix trust fund craft beer, health goth gochujang butcher master cleanse wolf venmo organic vexillologist. Chicharrones hella taxidermy crucifix, lomo next level plaid health goth cornhole pabst hot chicken meh poutine coloring book semiotics. Poutine mixtape tattooed marfa chicharrones roof party tumeric fingerstache schlitz pop-up. Health goth yr man bun pop-up banh mi fingerstache keffiyeh drinking vinegar lo-fi paleo. Paleo pok pok letterpress you probably haven't heard of them poutine edison bulb bushwick keffiyeh VHS austin celiac. Four dollar toast brooklyn swag, yr drinking vinegar twee gluten-free meh VHS 3 wolf moon craft beer vexillologist echo park whatever kogi.
          </p>
        </div>
      </div>
    </div>
  </section>

</template>

<script>

export default{
  mounted() {

    function loadJSON(callback) {   

      var xobj = new XMLHttpRequest();
      xobj.overrideMimeType("application/json");
      xobj.open('GET', 'my_data.json', true); 
      xobj.onreadystatechange = function () {
        if (xobj.readyState == 4 && xobj.status == "200") {
          try {
            var data = JSON.parse(xobj.responseText);
          } catch(err) {
            console.log('error')
            return;
          }
          callback(data);
        }
      };
      xobj.send(null);  
    }

    loadJSON(function(data) {
      console.log(data)
    });

  }
}

</script>

<style scoped>

div#wrap{
  width: 100%;
  display: grid;
}

div#leftPane{
  position: fixed;
  width: 25%;
  height: 100vh; 
  display: flex;
  justify-content: center;
  align-items: center;
}

div#stickyPane{
  padding: 50px;
}

div#stickyPane p#title{
  text-align: left;
  font-size: 2.25rem;
  background: #A3F3FD;
  display:inline;
  line-height: 3rem;
}

div#stickyPane p.meta{
  margin-top: 2rem;
  color: white; 
  letter-spacing: 1px;  
}

div#stickyPane p:last-child{
  margin-top: 0;
}

div#rightPane{
  position: absolute;
  width: 75%;
  left: 25%;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 50px 100px;  
}

div#mainText{
  max-width: 992px;
}

div#mainText img{
  width: 100%;
  margin-bottom:2rem;
}

div#mainText p, div#mainText ul, div#mainText ol, div#mainText li{
  margin-bottom: 2rem;
  font-size: 1.25rem;
  line-height: 2.25rem;
}

div#mainText li{
  margin-left: 3rem;
  margin-bottom: 1rem;
  letter-spacing: 1px;
}

div#mainText p:first-child{
  font-size: 2rem;
  font-weight: 600;

}

@media screen and (max-width: 767px) {
  div#leftPane{
    display: none;
  }
  div#rightPane{
    width: 100%;
    position: relative;
    left: 0;
    padding: 50px 30px;
  }
  div#mainText p, div#mainText ul, div#mainText ol, div#mainText li{
    font-size: 1rem;
  }
  div#mainText li{
    margin-left: 1rem;
  }
}

</style>