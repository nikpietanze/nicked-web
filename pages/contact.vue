<template>
    <div class="container mx-auto flex items-center justify-center h-max">
        <div class="rounded-lg border my-[5.5rem] bg-white text-gray-800 shadow-lg" data-v0-t="card">
            <div class="p-6">
                <form action="/api/contact" method="post" class="space-y-8">
                    <div class="space-y-2">
                        <h2 class="text-3xl font-semibold">Contact Us</h2>
                        <p class="text-zinc-500 dark:text-zinc-400">
                            Fill out the form below and we'll get back to you as soon as possible.
                        </p>
                    </div>
                    <div class="space-y-4">
                        <div class="space-y-2">
                            <label
                                class="text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70"
                                for="email">
                                Email
                            </label>
                            <input
                                class="flex h-10 w-full rounded-md border border-input bg-background px-3 py-2 text-sm ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50"
                                id="email" placeholder="Enter your email" type="email" />
                        </div>
                        <div class="space-y-2">
                            <label
                                class="text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70">
                                Contact Reason
                            </label>
                            <select
                                class="bg-[url('/static/img/down-arrow.svg')] bg-no-repeat bg-[98%_center] cursor-pointer flex h-10 w-full items-center justify-between rounded-md border appearance-none px-3 py-2 text-sm ring-offset-background placeholder:text-muted-foreground focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50">
                                <option value="issue">Technical Issue</option>
                                <option value="feedback">Product Feedback</option>
                            </select>
                        </div>
                        <div class="space-y-2">
                            <label
                                class="text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70"
                                for="message">
                                Message
                            </label>
                            <textarea
                                class="flex w-full rounded-md border border-input bg-background px-3 py-2 text-sm ring-offset-background placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50 min-h-[100px]"
                                id="message" placeholder="Enter your message"></textarea>
                        </div>
                        <button
                            class="inline-flex items-center justify-center rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 hover:bg-primary/90 h-10 px-4 py-2 bg-gray-800 text-white"
                            type="submit">
                            Send message
                        </button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>
