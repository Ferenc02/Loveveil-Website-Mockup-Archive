<script>
	import locked_app_image from '$lib/images/locked_app.png';
	import unlocked_app_image from '$lib/images/unlocked_app.png';
	import chat_app_image from '$lib/images/chat_app.png';
	import unlocked_chat_image from '$lib/images/chat_unlocked_app.png';
	import profile_image from '$lib/images/profile_app.png';

	import Donate from '../Donate.svelte';
</script>

<svelte:head>
	<title>Decoding LoveVeil: Exploring How the App Works and Its Exciting Features</title>
	<meta
		name="description"
		content="Explore LoveVeil's mechanics and anticipated features. From blurred images to engaging chats, uncover the essence of our app's authentic connection-building approach."
	/>
	<meta property="og:image" content={locked_app_image} />
	<meta property="og:image" content={unlocked_app_image} />
</svelte:head>

<hgroup>
	<h1>LoveVeil App Mechanics and Features</h1>
	<div class="text_container">
		<p>
			Welcome to a deeper understanding of LoveVeil's inner mechanics and features. Explore the
			intricate details that make our app unique and effective in fostering authentic connections.
			From innovative image unveiling to engaging conversations, discover how LoveVeil redefines the
			way you connect and build relationships.
		</p>
		<div class="images image_inherit">
			<img src={locked_app_image} alt="locked app" class="image_inherit mini_hover" />
			<img src={unlocked_app_image} alt="locked app" class="image_inherit mini_hover" />
		</div>
	</div>
	<article>
		<h2>Image Unveiling</h2>
		<div class="text_container split">
			<div>
				<p>
					Experience a refreshing twist in the dating world with our Image Unveiling feature. This
					innovative approach sparks curiosity by utilizing softly blurred images that transition to
					clear as connections deepen.
				</p>

				<p>
					When exploring profiles, you'll encounter images that leave a hint of mystery, inviting
					you to delve into conversations. As interactions progress, images will unlock, creating an
					exciting journey of discovery, enhancing the anticipation of getting to know someone on a
					deeper level.
				</p>

				<p>
					Loveveil symbolizes our commitment to authentic connections that transcend appearances. By
					focusing on conversations first, we invite users to forge bonds rooted in shared interests
					and genuine interactions instead of focusing only on appearances.
				</p>
			</div>
			<img src={locked_app_image} alt="locked app" class="image_inherit mini_hover" />
		</div>
	</article>
	<article>
		<h2>Conversation Emphasis</h2>

		<div class=" text_container split reverse">
			<img src={chat_app_image} alt="chat section in the app" class="image_inherit mini_hover" />
			<div>
				<p>
					LoveVeil reimagines the dating landscape by placing conversations at the forefront of
					forging connections. This intentional shift transforms the way users interact, encouraging
					meaningful exchanges that delve into shared interests and values.
				</p>

				<p>
					By fostering conversations that go beyond surface-level small talk, LoveVeil opens the
					door to authentic connections. Users are prompted to engage in discussions that revolve
					around their passions and experiences, setting the stage for connections that are based on
					more than just initial impressions.
				</p>

				<p>
					This philosophy nurtures connections that are rooted in understanding, compatibility, and
					shared experiences. By prioritizing conversations, LoveVeil cultivates a community where
					users are free to express themselves and forge connections that have the potential to
					deepen into something truly meaningful.
				</p>
			</div>
		</div>
	</article>
	<article>
		<h2>Progressive Unblur</h2>
		<div class="text_container split">
			<div>
				<p>
					The app introduces an element of anticipation with its Progressive Unblur feature. As
					conversations between users evolve, so does the visual experience. When browsing profiles,
					you'll notice that images start in a softly blurred state. However, as conversations
					unfold and connections deepen, these images will transition from blurred to clear.
				</p>

				<p>
					This unique process adds a touch of excitement, allowing users to explore not only each
					other's personalities through conversations but also to experience a gradual unblur of
					their visual profiles. This innovative approach fosters a dynamic and engaging journey,
					encouraging users to invest time and attention in building connections that align on both
					emotional and visual levels.
				</p>

				<p>
					With Progressive Unblur, LoveVeil creates an intriguing and immersive connection-building
					experience that's unlike any other dating app. This feature encapsulates the essence of
					LoveVeil's philosophy – Love Beyond the Surface LoveVeil Where Blur Blossoms into True
					Connection.
				</p>
			</div>

			<img
				src={unlocked_chat_image}
				alt="unlocked section of the person app"
				class="image_inherit mini_hover"
			/>
		</div>
	</article>
	<article>
		<h2>Interactive Profiles</h2>

		<div class="text_container split reverse">
			<img src={profile_image} alt="locked app" class="image_inherit mini_hover" />
			<div>
				<p>
					LoveVeil redefines the dating landscape with its Interactive Profiles, where depth and
					personality take center stage. Beyond the standard profile pictures, users have the
					opportunity to showcase their unique interests, hobbies, and values. Interactive prompts
					and sections enable users to share their favorite books, travel destinations, music
					genres, and more.
				</p>

				<p>
					This feature enriches conversations by offering potential conversation starters that go
					beyond the usual introductory topics. When engaging with a user's profile, you'll find a
					vibrant tapestry of their personality and preferences, sparking connections that resonate
					on a deeper level.
				</p>

				<p>
					LoveVeil's commitment to fostering authentic bonds is encapsulated in its Interactive
					Profiles, creating a space where users can truly get to know each other beyond the
					surface. With each interaction, you'll gain insights into what makes someone tick, setting
					the stage for more meaningful and engaging conversations.
				</p>
			</div>
		</div>
	</article>
	<article>
		<h2>In-App Messaging</h2>
		<div class="text_container split">
			<div>
				<p>
					At LoveVeil, conversations are at the heart of building meaningful connections. Our in-app
					messaging system is designed to provide a seamless and engaging communication experience
					that goes beyond the standard. When you connect with someone, you're entering a space
					where you can explore shared interests, exchange thoughts, and truly get to know each
					other.
				</p>

				<p>
					The messaging platform is user-friendly and intuitive, allowing you to send and receive
					messages effortlessly. You can send text or voice messages and even use emojis to express
					your thoughts and emotions. In addition, you can easily access your message history to
					revisit past conversations, helping you maintain continuity in your connections.
				</p>

				<p>
					Whether you're engaging in a lighthearted conversation about your favorite books or
					discussing profound life experiences, LoveVeil's in-app messaging platform provides the
					foundation for genuine interactions. It's a space where connections are nurtured,
					conversations flourish, and relationships evolve – all while maintaining the utmost
					privacy and security for our users.
				</p>
			</div>
			<img src={chat_app_image} alt="chat section in the app" class="image_inherit mini_hover" />
		</div>
	</article>
	<article class="donate_container">
		<Donate />
	</article>
</hgroup>

<style lang="scss">
	h1 {
		padding-bottom: 1rem;
	}
	h2 {
		padding: 1rem;
	}
	p {
		font-weight: 300;
		font-size: 1.2rem;
	}

	.text_container {
		display: flex;
		flex-wrap: wrap;

		justify-content: center;

		img {
			max-height: 40rem;
		}
		.images {
			display: flex;
			flex-wrap: wrap;
			flex-direction: row;

			margin: 1rem;
			justify-content: center;
		}
	}

	.split {
		flex-direction: row;

		div {
			display: flex;
			flex-direction: column;
			@media screen and (min-width: 1300px) {
				justify-content: space-between;
				width: 70%;
				padding: 2rem;
				justify-content: space-around;
			}
		}
		p {
			padding: 1rem;
			@media screen and (min-width: 1300px) {
				padding: 2rem;
			}
		}
		img {
			@media screen and (min-width: 1300px) {
				margin-right: 6rem;
			}
		}
	}
	.reverse {
		flex-wrap: wrap-reverse;
		img {
			@media screen and (min-width: 1300px) {
				margin-left: 6rem;
				margin-right: 0;
			}
		}
	}
	.donate_container {
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 0.5rem;
	}
</style>
