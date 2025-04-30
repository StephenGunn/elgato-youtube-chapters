<section class="how-to-use" id="how-to-use">
	<h2>Setup Guide &amp; How To Use</h2>
	<p class="caveat">
		This workflow isn't perfect and a bit of a hack, but it works for me. I hope it helps you too!
	</p>
	<div class="step-by-step">
		<div class="step">
			<h3>Step 1: Set Up the Timestamp Plugin</h3>
			<p>
				The
				<a
					href="https://marketplace.elgato.com/product/timestamp-76bd699e-cded-44d8-aaa5-a7e863657b93"
					>Elgato Timestamp plugin</a
				>
				lets you mark memorable events with a simple key press, perfect for creating YouTube chapters:
			</p>
			<img src="/timestamp.png" alt="Elgato Stream Deck with Timestamp Plugin" />
			<ol>
				<li>
					Install the
					<a
						href="https://marketplace.elgato.com/product/timestamp-76bd699e-cded-44d8-aaa5-a7e863657b93"
						>official Timestamp plugin from the Stream Deck Marketplace</a
					>
				</li>
				<li>Add the "New Log" action to start tracking timestamps</li>
				<li>Add the "Marker" action to mark key moments during your stream</li>
				<li>Make sure "Elapsed time" is checked in the Marker settings</li>
			</ol>
		</div>

		<div class="step">
			<h3>Step 2: Create Multi-Actions for Show or Stream Segments</h3>
			<p>
				For streamlined workflow, create Multi-Actions that both change your scene and mark
				timestamps:
			</p>
			<img src="/multiaction.png" alt="An example of a multi-action in OBS" />
			<ol>
				<li>Create a new Multi-Action button on your Stream Deck</li>
				<li>Add your scene switching action (e.g., "OBS Studio: Scene")</li>
				<li>Add the "Timestamp: Marker" action to the same Multi-Action</li>
				<li>Set a descriptive title for the marker (e.g., "Guest Introduction", "Q&A Session")</li>
				<li>Repeat for each segment of your show</li>
			</ol>
			<p>
				This allows you to simultaneously switch scenes and mark timestamps with a single button
				press.
			</p>
		</div>

		<div class="step">
			<h3>Step 3: During Your Stream</h3>
			<p>While streaming, use your Stream Deck to mark important segments:</p>
			<img src="/view.png" alt="The dual streamdeck setup I use to run shows" />
			<ol>
				<li>
					Don't forget to press the "New Log" button at the beginning of your stream, or your
					timestamps won't get logged!
				</li>
				<li>You'll also want to</li>
				<li>
					As your show progresses, press your Multi-Action buttons to switch scenes and mark
					timestamps
				</li>
				<li>Each press creates a timestamp with your pre-defined label</li>
				<li>Continue marking all important segments throughout your stream</li>
			</ol>
		</div>

		<div class="step">
			<h3>Step 4: Check Your Timestamps</h3>
			<p>After your stream is complete:</p>
			<ol>
				<li>Press the "New Log" button again to end the logging session (important)</li>
				<li>Your timestamp log will be saved as a .txt file in the directory you set up</li>
				<li>
					The log file will contain lines like:<br />
					<code>elapsed time: 00:02:39 text: Last Week's Episode</code>
				</li>
			</ol>
		</div>

		<div class="step">
			<h3>Step 5: Convert to YouTube Chapters</h3>
			<p>Use our converter to transform your timestamps to YouTube-compatible chapter markers:</p>
			<ol>
				<li>Drag and drop your timestamp file into the converter</li>
				<li>The first chapter will be set to 00:00 (YouTube requirement)</li>
				<li>
					If there is no timestamp in the first 10 seconds of your log, a generic "Intro" chapter
					will be created
				</li>
				<li>Adjust the offset if needed (see below)</li>
				<li>Copy the formatted chapters</li>
				<li>Paste into your YouTube video description</li>
			</ol>
		</div>
	</div>

	<div class="offset-explanation">
		<h3>Why You Might Need the Offset Feature</h3>
		<p>The offset feature is essential for streamers because:</p>
		<ul>
			<li>
				<strong>Stream Start Timing:</strong> The exact moment you go live often doesn't match when you
				start your timestamp log
			</li>
			<li>
				<strong>Editing Adjustments:</strong> If you trim portions of your video before uploading to
				YouTube
			</li>
			<li>
				<strong>Added Content:</strong> If you add an intro to your video that wasn't in the original
				stream
			</li>
			<li>
				<strong>VOD vs. Stream:</strong> Differences between your live stream and the final video on
				demand
			</li>
		</ul>

		<h4>How to Use the Offset:</h4>
		<ul>
			<li>
				<strong>Positive Offset:</strong> Moves all timestamps later (e.g., +5 seconds if you added a
				5-second intro)
			</li>
			<li>
				<strong>Negative Offset:</strong> Moves all timestamps earlier (e.g., -10 seconds if you trimmed
				the first 10 seconds)
			</li>
			<li>
				Use the preset buttons for quick adjustments or enter a specific value for precise control
			</li>
			<li>The first chapter will always remain at 00:00 as required by YouTube</li>
		</ul>
	</div>

	<div class="plugin-benefits">
		<h3>Benefits of Using the Timestamp Plugin with Our Converter</h3>
		<p>
			The Elgato Timestamp plugin paired with our converter offers streamers several advantages:
		</p>
		<ul>
			<li>
				<strong>Real-time Marking:</strong> Mark every moment during your live stream without disrupting
				your flow
			</li>
			<li>
				<strong>Time Saving:</strong> No more scrubbing through recordings or scribbling notes
			</li>
			<li>
				<strong>Workflow Integration:</strong> Combine scene switching and timestamp marking with Multi-Actions
			</li>
			<li>
				<strong>Format Conversion:</strong> Automatically convert from Elgato's format to YouTube's required
				format
			</li>
			<li>
				<strong>Fine-Tuning:</strong> Adjust timestamps with precise offset controls to match your final
				video
			</li>
		</ul>
		<p>
			I created this tool to help my own workflow. I understand it might not work for everyone.
			Please feel free to reach out with any comments or suggestions.
		</p>
	</div>
</section>

<style>
	.how-to-use {
		max-width: 1200px;
		margin: 0 auto;
		padding: 2rem;
		line-height: 1.6;
	}

	.how-to-use h2 {
		font-size: var(--fs-xl);
		color: var(--primary);
		margin-bottom: 2rem;
		text-align: center;
		border-bottom: 2px dashed var(--border);
		padding-bottom: 1rem;
		letter-spacing: -2.5px;
		padding: 0 2rem;
	}

	.step-by-step {
		display: grid;
		gap: 3rem;
		margin-bottom: 3rem;
	}

	.step {
		background: var(--border);
		border-radius: 8px;
		padding: 2rem;
		box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
		position: relative;
		border-left: 4px solid var(--accent);
	}

	.step h3 {
		font-size: var(--fs-lg);
		color: var(--primary);
		margin-top: 0;
		margin-bottom: 1.5rem;
		display: flex;
		align-items: center;
	}

	.step h3::before {
		content: '';
		width: 30px;
		height: 30px;
		background: var(--accent);
		border-radius: 50%;
		margin-right: 1rem;
		display: flex;
		align-items: center;
		justify-content: center;
		flex-shrink: 0;
	}

	.step p {
		font-size: var(--fs-base);
		margin-bottom: 1.5rem;
	}

	.step img {
		width: 100%;
		max-width: 600px;
		border-radius: 8px;
		margin: 1.5rem auto;
		display: block;
		border: 2px solid var(--secondary);
	}

	.step ol {
		padding-left: 1.5rem;
		margin-bottom: 1.5rem;
	}

	.step ol li {
		margin-bottom: 0.75rem;
		padding-left: 0.5rem;
	}

	.step code {
		background: rgba(147, 186, 228, 0.15);
		padding: 0.2rem 0.4rem;
		border-radius: 4px;
		font-family: monospace;
		font-size: 0.9em;
	}

	/* Section specific styling */
	.offset-explanation,
	.plugin-benefits {
		background: linear-gradient(135deg, var(--border), rgba(21, 80, 145, 0.3));
		border-radius: 8px;
		padding: 2rem;
		margin-bottom: 3rem;
		box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
	}

	.offset-explanation h3,
	.plugin-benefits h3 {
		font-size: var(--fs-lg);
		color: var(--primary);
		margin-top: 0;
		margin-bottom: 1.5rem;
		border-bottom: 1px solid var(--secondary);
		padding-bottom: 0.75rem;
	}

	.offset-explanation h4 {
		font-size: var(--fs-md);
		color: var(--primary);
		margin: 1.5rem 0 1rem;
	}

	.offset-explanation ul,
	.plugin-benefits ul {
		list-style-type: none;
		padding-left: 0;
	}

	.offset-explanation ul li,
	.plugin-benefits ul li {
		margin-bottom: 1rem;
		position: relative;
		padding-left: 1.8rem;
	}

	.offset-explanation ul li::before,
	.plugin-benefits ul li::before {
		content: '•';
		color: var(--accent);
		font-size: 1.5em;
		position: absolute;
		left: 0;
		top: -0.2rem;
	}

	.offset-explanation strong,
	.plugin-benefits strong {
		color: var(--primary);
	}

	@media (min-width: 768px) {
		.step-by-step {
			grid-template-columns: repeat(2, 1fr);
		}

		.step:first-child {
			grid-column: 1 / -1;
		}
	}

	@media (min-width: 1024px) {
		.step-by-step {
			grid-template-columns: repeat(2, 1fr);
		}
	}

	.step {
		transition:
			transform 0.3s ease,
			box-shadow 0.3s ease;
	}

	.plugin-benefits p:last-child {
		font-size: var(--fs-md);
		text-align: center;
		margin-top: 2rem;
		font-style: italic;
		color: var(--primary);
	}

	.caveat {
		font-size: var(--fs-sm);
		color: var(--text);
		text-align: center;
		margin-bottom: 2rem;
	}
</style>
