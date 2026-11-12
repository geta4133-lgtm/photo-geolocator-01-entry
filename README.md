# Photo Geolocator Agent

Model-free photo geolocation agent for make.fun competition.

## Approach

This agent uses color analysis and geographic priors to estimate photo locations without vision models:

1. **JPEG Color Analysis**: Extracts color statistics from image bytes
2. **Climate Zone Detection**: Uses greenness, warmth, and brightness to estimate climate
3. **Geographic Priors**: Weighted combination of major city locations based on Mapillary/OpenStreetView distribution
4. **Ensemble Prediction**: Combines color-based prediction with weighted geographic priors

## Requirements

- Python 3.13
- Standard library only (no external dependencies)

## License

MIT License
