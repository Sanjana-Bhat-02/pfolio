<script>
    import { onMount } from "svelte";
    import Header from "../components/Header.svelte";
    import Footer from "../components/Footer.svelte";
    let particlesConfig = {
        particles: {
            number: {
                value: 80,
                density: {
                    enable: true,
                    value_area: 800,
                },
            },
            color: {
                value: "#ffffff",
            },
            shape: {
                type: "circle",
                stroke: {
                    width: 0,
                    color: "#000000",
                },
                polygon: {
                    nb_sides: 5,
                },
                image: {
                    src: "img/github.svg",
                    width: 100,
                    height: 100,
                },
            },
            opacity: {
                value: 0.5,
                random: false,
                anim: {
                    enable: false,
                    speed: 1,
                    opacity_min: 0.1,
                    sync: false,
                },
            },
            size: {
                value: 3,
                random: true,
                anim: {
                    enable: false,
                    speed: 40,
                    size_min: 0.1,
                    sync: false,
                },
            },
            line_linked: {
                enable: true,
                distance: 150,
                color: "#ffffff",
                opacity: 0.4,
                width: 1,
            },
            move: {
                enable: true,
                speed: 6,
                direction: "none",
                random: false,
                straight: false,
                out_mode: "out",
                bounce: false,
                attract: {
                    enable: false,
                    rotateX: 600,
                    rotateY: 1200,
                },
            },
        },
        interactivity: {
            detect_on: "canvas",
            events: {
                onhover: {
                    enable: true,
                    mode: "repulse",
                },
                onclick: {
                    enable: true,
                    mode: "push",
                },
                resize: true,
            },
            modes: {
                grab: {
                    distance: 400,
                    line_linked: {
                        opacity: 1,
                    },
                },
                bubble: {
                    distance: 400,
                    size: 40,
                    duration: 2,
                    opacity: 8,
                    speed: 3,
                },
                repulse: {
                    distance: 200,
                    duration: 0.4,
                },
                push: {
                    particles_nb: 4,
                },
                remove: {
                    particles_nb: 2,
                },
            },
        },
        retina_detect: true,
    };

    onMount(() => {
        const script = document.createElement("script");
        script.src =
            "https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js";
        script.onload = () => {
            particlesJS("particles-js", particlesConfig);
        };

        document.head.appendChild(script);
    });
</script>

<div class="wrapper">
    <div id="particles-js" class="bg-zinc-900" />
    <Header />
    <div class="con">
        <div class="sign">
            <span class="fast-flicker">Hey&nbsp;</span>There!&nbsp;<span
                class="flicker">I'm&nbsp;</span
            >Sanjana
        </div>
    </div>

    <div class="subtitle">
        <p>Aspiring</p>
        <p>Frontend</p>
        <p>Developer</p>
    </div>
    <Footer />
</div>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Poppins&display=swap");
    .subtitle {
        margin-top: 20px;
        display: flex;
        color: white;
    }
    .wrapper {
        position: relative;
        height: 100vh;
    }

    #particles-js {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: 0;
        background-attachment: fixed;
    }

    .con {
        font-size: 100%;
        position: relative;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
        margin-top: 40px;
    }

    .sign {
        position: absolute;
        display: flex;
        justify-content: center;
        align-items: center;
        width: 50%;
        height: 50%;
        background-image: radial-gradient(
            ellipse 50% 35% at 50% 50%,
            #6b1839,
            transparent
        );
        transform: translate(-50%, -50%);
        letter-spacing: 2;
        left: 50%;
        top: 50%;
        font-family: "Poppins";
        text-transform: uppercase;
        font-size: 3em;
        color: #ffe6ff;
        text-shadow: 0 0 0.6rem #ffe6ff, 0 0 1.5rem #ff65bd,
            -0.2rem 0.1rem 1rem #ff65bd, 0.2rem 0.1rem 1rem #ff65bd,
            0 -0.5rem 2rem #ff2483, 0 0.5rem 3rem #ff2483;
        animation: shine 2s forwards, flicker 3s infinite;
    }

    p {
        color: white;
        font-size: 2em;
        position: absolute;
        top: 100%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
    @keyframes blink {
        0%,
        22%,
        36%,
        75% {
            color: #ffe6ff;
            text-shadow: 0 0 0.6rem #ffe6ff, 0 0 1.5rem #ff65bd,
                -0.2rem 0.1rem 1rem #ff65bd, 0.2rem 0.1rem 1rem #ff65bd,
                0 -0.5rem 2rem #ff2483, 0 0.5rem 3rem #ff2483;
        }
        28%,
        33% {
            color: #ff65bd;
            text-shadow: none;
        }
        82%,
        97% {
            color: #ff2483;
            text-shadow: none;
        }
    }

    .flicker {
        animation: shine 2s forwards, blink 3s 2s infinite;
    }

    .fast-flicker {
        animation: shine 2s forwards, blink 10s 1s infinite;
    }

    @keyframes shine {
        0% {
            color: #6b1839;
            text-shadow: none;
        }
        100% {
            color: #ffe6ff;
            text-shadow: 0 0 0.6rem #ffe6ff, 0 0 1.5rem #ff65bd,
                -0.2rem 0.1rem 1rem #ff65bd, 0.2rem 0.1rem 1rem #ff65bd,
                0 -0.5rem 2rem #ff2483, 0 0.5rem 3rem #ff2483;
        }
    }

    @keyframes flicker {
        from {
            opacity: 1;
        }

        4% {
            opacity: 0.9;
        }

        6% {
            opacity: 0.85;
        }

        8% {
            opacity: 0.95;
        }

        10% {
            opacity: 0.9;
        }

        11% {
            opacity: 0.922;
        }

        12% {
            opacity: 0.9;
        }

        14% {
            opacity: 0.95;
        }

        16% {
            opacity: 0.98;
        }

        17% {
            opacity: 0.9;
        }

        19% {
            opacity: 0.93;
        }

        20% {
            opacity: 0.99;
        }

        24% {
            opacity: 1;
        }

        26% {
            opacity: 0.94;
        }

        28% {
            opacity: 0.98;
        }

        37% {
            opacity: 0.93;
        }

        38% {
            opacity: 0.5;
        }

        39% {
            opacity: 0.96;
        }

        42% {
            opacity: 1;
        }

        44% {
            opacity: 0.97;
        }

        46% {
            opacity: 0.94;
        }

        56% {
            opacity: 0.9;
        }

        58% {
            opacity: 0.9;
        }

        60% {
            opacity: 0.99;
        }

        68% {
            opacity: 1;
        }

        70% {
            opacity: 0.9;
        }

        72% {
            opacity: 0.95;
        }

        93% {
            opacity: 0.93;
        }

        95% {
            opacity: 0.95;
        }

        97% {
            opacity: 0.93;
        }

        to {
            opacity: 1;
        }
    }

    @media (max-width: 768px) {
        .sign {
            flex-direction: column;
        }
    }
</style>
