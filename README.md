<h1>Marlin as deployed on my 3D printers</h1>
<h3>Please use the official Marlin</h3>
<p>This repo was forked here so that I could make changes quickly, build in Gitpod test and deploy rapidly</p>
<p>Branch SPRITE is for Ender 3 with Sprite Pro, linear X rail, CR Touch and SKR E3 Turbo</p>

<p>Master is for Ender 3 with stock hot end, linear x rail, Tronxy TR sensor and SKR E3 Turbo </p>

<h3>Code changes over Marlin:</h3>
<ul>Added status screen update for G28 start and end since z homing takes a while and it's hard to tell with the leadscrews if the printer is actually doing something.</ul>

<p>To build, use gitpod:</p>
<pre>
git checkout SPRITE
python3 -c "$(curl -fsSL https://raw.githubusercontent.com/platformio/platformio/master/scripts/get-platformio.py)"
/home/gitpod/.platformio/penv/bin/platformio run
</pre>

