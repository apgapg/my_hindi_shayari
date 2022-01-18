<script lang="ts">
    const datas = [
        "क्या बात करें तेरे आखों की\nएक जेल है बिन सलाखों की",
        "मेरे दामन में काटों के सिवा कुछ भी नहीं\n" +
        "आप फूलों के खरीदार नजर आते हैं",
        "हर घूंट में तेरी यादें बसीं हैं\n" + "केसे कह दूँ, शराब कड़वी है",
        "बेच दूँ क्या सारी परेशानियां?\n" + "मौत अछा दाम दे रहीं है",
        "थोड़ा इंतजार तो कर लेते\n" + "दिल नहीं, मेरे दिन खराब थे",
        "तुमारी याद, जेसे बारिश की वो बूँद,\n" +
        "जो मेहसूस तो होती है,\n" +
        "पर पकड़ने पर अपना अस्तित्व खो देती है",
        "पानी मे तेरा अक्स देख कर इतरा रहा था मैं,\n" +
        "किसी ने पत्थर फेंककर, मंज़र बदल दिया",
    ];
</script>

<main class="bg-zinc-800 h-screen">
    <div class="flex items-center p-3 px-4">
        <div
                class="text-white text-2xl text-left font-semibold tracking-wider "
                style="font-family: 'Caveat', cursive;"
        >
            Hindi Shayari
        </div>
        <div class="flex-1"></div>
        <a class="hover:bg-zinc-600 rounded-full h-8 w-8" href="https://github.com/apgapg" target="_blank">
          <i class="fab fa-github text-white text-2xl cursor-pointer "></i>
        </a>
<div class="mx-2"></div>
        <a class="hover:bg-zinc-600 rounded-full h-8 w-8" href="https://twitter.com/ayushpgupta" target="_blank">
          <i class="fab fa-twitter text-white text-2xl cursor-pointer "></i>
        </a>


    </div>
    <div class=" bg-zinc-300 opacity-20 border-b"></div>

    <div class="flex flex-wrap justify-center p-4 gap-4 overflow-y-auto">
        {#each datas as data}
            <div
                    class="bg-zinc-700 overflow-hidden text-white shadow border border-zinc-600 text-center text-lg rounded-lg"
            >
                <img
                        src="https://picsum.photos/300/200?random={datas.indexOf(data) + 2}"
                        class="object-fill h-48 w-full"
                        alt="img"
                />
                <pre class="px-3 py-4 font-medium">
   {data}
  </pre>
            </div>
        {/each}
    </div>
</main>

<style>
    :root {
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
        Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
        @apply bg-zinc-800;
    }

    main {
        text-align: center;
        margin: 0 auto;
    }

    h1 {
        color: #ff3e00;
        text-transform: uppercase;
        font-size: 4rem;
        font-weight: 100;
        line-height: 1.1;
        margin: 2rem auto;
        max-width: 14rem;
    }

    p {
        max-width: 14rem;
        margin: 1rem auto;
        line-height: 1.35;
    }

    @media (min-width: 480px) {
        h1 {
            max-width: none;
        }

        p {
            max-width: none;
        }
    }
</style>
