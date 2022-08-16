                                                        

<template>
    <div class='container my-4'>
        <div class="d-flex justify-content-between align-items-center">
            <h5>Reviews: 
                <span class="badge bg-dark rounded-pill">
                    {{store.reviewsLength}}
                </span>
            </h5>
            <h5>Average: 
                <span class="badge bg-warning text-dark rounded-pill">
                    {{ store.calculateReviewsAverage }}
                </span>
            </h5>
        </div>
    </div>
</template>

<script setup>
    import {useReviewStore} from '../stores'

    //get store
    const store = useReviewStore();
</script>

<style>
</style>
                                                        
                                                    